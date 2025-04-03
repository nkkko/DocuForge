# DocuForge AI Architecture

## Overview

DocuForge AI employs a modular architecture with several core components designed to support documentation-first development with AI assistance.

```
┌─────────────────┐      ┌────────────────────┐      ┌─────────────────┐
│ Browser Editor  │◄────►│ Backend Services   │◄────►│ Git Repository  │
└─────────────────┘      └────────────────────┘      └─────────────────┘
        ▲                         ▲                           ▲
        │                         │                           │
        ▼                         ▼                           │
┌─────────────────┐      ┌────────────────────┐              │
│ Visual Canvas   │◄────►│ AI Assistant       │              │
└─────────────────┘      └────────────────────┘              │
        ▲                         ▲                           │
        │                         │                           │
        ▼                         │                           ▼
┌─────────────────┐      ┌────────────────────┐    ┌─────────────────┐
│ Documentation   │◄────►│ LLMs.txt Generator │    │ Rendered Docs   │
│ Renderer        │      └────────────────────┘    │ (Static Site)   │
└─────────────────┘                                └─────────────────┘
```

## Core Components

- [Document Editor Service](./document-editor.md): Browser-based rich text editing with markdown conversion
- [Documentation Organization System](./organization-system.md): Visual canvas for structuring documentation
- [Version Control Integration](./version-control.md): Git-based storage and version tracking
- [Metadata Management System](./metadata-management.md): Tagging, versioning, and ownership tracking
- [AI Assistant Engine](./ai-assistant.md): Documentation improvement and code generation capabilities
- [Documentation Rendering Engine](./rendering-engine.md): Beautiful documentation generation
- [Project Management Integration](./project-management.md): ShapeUp methodology implementation
- [LLMs.txt Generation Service](./llms-txt-generator.md): Automatic creation of LLM-friendly documentation exports

## Technology Stack

### Frontend
- React with TypeScript (Component reusability, strong ecosystem)
- TipTap editor (Open-source, extensible, Prosemirror-based)
- React Flow for canvas visualization (Powerful node-edge visualization)
- Tailwind CSS (Rapid UI development, consistent styling)

### Backend
- Node.js with Express (JavaScript consistency across stack, developer productivity)
- GraphQL API (Flexible querying for complex document relationships)
- Prisma ORM (Type-safe database access, schema migrations)

### Database
- PostgreSQL (Relational data with JSON support for document metadata)
- Redis for caching (Performance for real-time collaboration)

### AI Components
- Fine-tuned LLM based on open-source model (Proprietary advantage, cost control)
- Vector database (Pinecone or Weaviate) for semantic search (Efficient similarity search)
- LangChain for LLM orchestration (Simplified AI integration workflows)

### DevOps
- Docker and Docker Compose (Consistent development and deployment)
- GitHub Actions for CI/CD (Tight integration with Git repository)
- Serverless deployment where appropriate (Cost-effective scaling)

### Documentation Generation
- MDX support (Interactive documentation components)
- Next.js for static site generation (Performance, SEO, flexibility)
