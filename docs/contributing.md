# Contributing to DocuForge AI

## Welcome!

Thank you for considering contributing to DocuForge AI. This document provides guidelines and instructions for contributing to the project.

## Ways to Contribute

### Documentation

- Improve existing documentation
- Add missing documentation
- Create tutorials and examples
- Translate documentation

### Code

- Fix bugs
- Implement new features
- Improve performance
- Add tests

### Design

- Improve user interface
- Create icons and illustrations
- Design documentation themes

### Community

- Answer questions
- Report bugs
- Suggest features
- Share success stories

## Development Setup

1. **Fork the repository**

2. **Clone your fork**
   ```bash
   git clone https://github.com/your-username/docuforge.git
   cd docuforge
   ```

3. **Install dependencies**
   ```bash
   npm install
   ```

4. **Setup the database**
   ```bash
   docker-compose up -d postgresql redis
   npm run db:migrate
   ```

5. **Start the development server**
   ```bash
   npm run dev
   ```

## Development Workflow

### Branch Naming

- `feature/short-description` for new features
- `fix/short-description` for bug fixes
- `docs/short-description` for documentation changes

### Commit Messages

Follow the conventional commits format:

```
<type>(<scope>): <short summary>

<body>

<footer>
```

Types: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`

### Testing

All contributions should include appropriate tests:

```bash
# Run all tests
npm test

# Run a specific test
npm test -- -t "test name"

# Run tests in watch mode
npm test -- --watch
```

### Code Style

This project uses ESLint and Prettier for code formatting. Run linters before submitting a PR:

```bash
npm run lint
```

## Pull Request Process

1. **Create a branch** from the `main` branch
2. **Make your changes** and commit them
3. **Add tests** for new features or bug fixes
4. **Update documentation** as needed
5. **Run tests** to ensure they pass
6. **Submit a pull request** to the `main` branch
7. **Address review comments** if any

## Documentation Guidelines

### Style

- Use clear, concise language
- Follow the documentation structure
- Include examples where appropriate
- Use proper markdown formatting

### Format

- Files should use `.md` extension
- Follow the existing folder structure
- Add links to related documentation

## Community Guidelines

- Be respectful and inclusive
- Provide constructive feedback
- Help others when possible
- Follow the code of conduct

## Questions?

If you have questions about contributing, please reach out to the maintainers or open an issue on GitHub.

---

Thank you for contributing to DocuForge AI! Your efforts help make documentation-first development better for everyone.
