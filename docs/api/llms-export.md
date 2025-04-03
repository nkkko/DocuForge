# LLMs Export API

## Overview

The LLMs Export API allows programmatic generation and management of LLMs.txt files and related expanded context files from project documentation.

## Types

```graphql
type LLMsExport {
  id: ID!
  projectId: ID!
  createdAt: DateTime!
  updatedAt: DateTime!
  config: LLMsConfig!
  files: [LLMsFile!]!
}

type LLMsFile {
  id: ID!
  exportId: ID!
  fileName: String!
  fileType: LLMsFileType!
  content: String!
  size: Int!
  createdAt: DateTime!
}

enum LLMsFileType {
  LLMS_TXT
  LLMS_CTX_TXT
  LLMS_CTX_FULL_TXT
  MARKDOWN
}

input LLMsConfigInput {
  title: String
  summary: String
  detailedDescription: String
  requiredSections: [LLMsSectionInput!]!
  optionalSections: [LLMsSectionInput!]
  generateExpandedContext: Boolean
  generateFullContext: Boolean
}

input LLMsSectionInput {
  documentId: ID!
  title: String
  description: String
  order: Int
}
```

## Queries

### Get LLMs Export

Retrieve details of a specific LLMs export.

```graphql
query GetLLMsExport($id: ID!) {
  llmsExport(id: $id) {
    id
    projectId
    createdAt
    updatedAt
    config {
      title
      summary
      detailedDescription
      requiredSections {
        documentId
        title
        description
        order
      }
      optionalSections {
        documentId
        title
        description
        order
      }
      generateExpandedContext
      generateFullContext
    }
    files {
      id
      fileName
      fileType
      content
      size
      createdAt
    }
  }
}
```

### List Project LLMs Exports

Retrieve all LLMs exports for a project.

```graphql
query ListProjectLLMsExports($projectId: ID!) {
  projectLLMsExports(projectId: $projectId) {
    id
    createdAt
    updatedAt
    files {
      fileName
      fileType
    }
  }
}
```

## Mutations

### Generate LLMs Export

Generate a new LLMs export for a project.

```graphql
mutation GenerateLLMsExport($input: GenerateLLMsExportInput!) {
  generateLLMsExport(input: $input) {
    id
    files {
      id
      fileName
      fileType
      content
      size
    }
  }
}

input GenerateLLMsExportInput {
  projectId: ID!
  config: LLMsConfigInput!
}
```

### Delete LLMs Export

Delete an existing LLMs export.

```graphql
mutation DeleteLLMsExport($id: ID!) {
  deleteLLMsExport(id: $id) {
    success
    message
  }
}
```

## Subscriptions

### LLMs Export Generation Progress

Receive real-time updates during LLMs export generation.

```graphql
subscription LLMsExportProgress($exportId: ID!) {
  llmsExportProgress(exportId: $exportId) {
    exportId
    status
    progress
    currentStep
    totalSteps
    message
  }
}
```

## Error Codes

| Code | Description |
|------|-------------|
| `INVALID_CONFIG` | The provided LLMs configuration is invalid |
| `PROJECT_NOT_FOUND` | The specified project does not exist |
| `DOCUMENT_NOT_FOUND` | A document specified in the configuration does not exist |
| `EXPORT_NOT_FOUND` | The specified export does not exist |
| `GENERATION_FAILED` | The export generation process failed |
