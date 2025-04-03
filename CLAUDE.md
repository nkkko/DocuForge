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

## Git Workflow
- Create a new branch for each feature or bug fix: `git checkout -b feature/feature-name`
- Make atomic, focused commits with descriptive messages
- Push changes to the remote repository: `git push origin feature/feature-name`
- Always commit changes after work is completed
- Create pull requests for code reviews
- Delete branches after they are merged

## Repository
- https://github.com/nkkko/DocuForge.git

## AI Assistant Rules
- Always commit changes after completing assigned work
- Create a new branch for each new feature implementation
- Run lint and type checking before committing code
- Follow documentation-first approach for all features
- Generate appropriate tests for new functionality