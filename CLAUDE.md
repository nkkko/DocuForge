# DocuForge AI - Claude Coding Guidelines

## Commands
- **Build**: `npm run dev` - Start development server
- **Test**: `npm test` - Run all tests
- **Single Test**: `npm test -- -t "test name"` - Run specific test
- **Lint**: `npm run lint` - Check code style
- **Type Check**: `npm run typecheck` - Verify TypeScript types

## Code Style
- **Imports**: Group by external, internal, then type imports
- **Formatting**: Use Prettier with 2-space indentation
- **Types**: Always use TypeScript with proper interfaces/types
- **Naming**:
  - React components: PascalCase
  - Functions/variables: camelCase
  - Files: kebab-case.tsx for components
- **Error Handling**: Use try/catch with typed errors
- **Documentation**: Add JSDoc comments for public APIs
- **Components**: Prefer functional components with hooks
- **State Management**: Use React context for global state

## Architecture
- Follow document-first development approach
- Maintain clear separation between UI and business logic
- Utilize the LLMs.txt export functionality for AI-friendly documentation

## Repository
- https://github.com/nkkko/docuforge.git