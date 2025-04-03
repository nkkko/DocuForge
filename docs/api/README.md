# DocuForge AI API Reference

## Overview

DocuForge AI provides a GraphQL API for interacting with the platform programmatically. This API enables integration with external tools, custom workflows, and automation.

## Authentication

All API requests require authentication using an API key or JWT token.

```graphql
headers {
  "Authorization": "Bearer YOUR_API_TOKEN"
}
```

## Base URL

```
https://api.docuforge.ai/graphql
```

## Core Resources

- [Projects](./projects.md): Create and manage documentation projects
- [Documents](./documents.md): Work with individual documentation files
- [Canvas](./canvas.md): Manage document organization and relationships
- [Users](./users.md): User management and permissions
- [LLMs Export](./llms-export.md): Generate and manage LLMs.txt exports
- [AI Assistance](./ai-assistance.md): Access AI-powered documentation features

## Example Queries

### Fetch Project Details

```graphql
query GetProject($id: ID!) {
  project(id: $id) {
    id
    name
    description
    documents {
      id
      title
      updatedAt
    }
  }
}
```

### Create a New Document

```graphql
mutation CreateDocument($input: CreateDocumentInput!) {
  createDocument(input: $input) {
    id
    title
    content
    createdAt
  }
}
```

## Rate Limits

API requests are subject to rate limiting:

- 100 requests per minute for standard accounts
- 1000 requests per minute for enterprise accounts

Rate limit headers are included in all responses:

```
X-RateLimit-Limit: 100
X-RateLimit-Remaining: 95
X-RateLimit-Reset: 1620000000
```

## Webhooks

DocuForge AI can send webhook notifications for events:

- Document created/updated/deleted
- Project created/updated/deleted
- LLMs.txt generation completed
- AI assistance tasks completed

See [Webhooks](./webhooks.md) for configuration details.

## SDKs

Official client libraries are available for:

- JavaScript/TypeScript
- Python
- Ruby
- Go

See [Client Libraries](./client-libraries.md) for installation and usage instructions.
