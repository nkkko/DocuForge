# DocuForge AI Components

## Overview

DocuForge AI is built with a modular component architecture that enables flexibility, maintainability, and extensibility. This section documents the key components of the system.

## Frontend Components

- [Document Editor](./document-editor.md): Rich text editor with markdown support
- [Visual Canvas](./visual-canvas.md): Documentation organization interface
- [Project Dashboard](./project-dashboard.md): Project management and overview
- [LLMs.txt Generator UI](./llms-txt-generator-ui.md): Interface for configuring and generating LLMs.txt files
- [Documentation Preview](./documentation-preview.md): Real-time preview of rendered documentation

## Backend Components

- [Document Service](./document-service.md): Document storage and retrieval
- [GraphQL API](./graphql-api.md): API for frontend-backend communication
- [Git Integration](./git-integration.md): Version control system integration
- [AI Service](./ai-service.md): AI-powered assistance and generation
- [Rendering Service](./rendering-service.md): Documentation site generation

## Data Models

- [Document Model](./document-model.md): Structure of documentation entities
- [Project Model](./project-model.md): Organization of documents in projects
- [User Model](./user-model.md): User information and permissions
- [Metadata Model](./metadata-model.md): Tagging and classification system

## Integration Points

DocuForge AI provides several integration points for extending functionality:

- Custom editor extensions
- Theme customization
- Export format plugins
- External service webhooks
- AI model customization
- LLMs.txt format extensions

For details on extending DocuForge AI, see the [Extension Guide](./extension-guide.md).
