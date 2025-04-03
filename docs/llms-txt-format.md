# LLMs.txt Format

## Overview

The LLMs.txt format is a standardized way to provide information to help large language models (LLMs) better understand and interact with websites, repositories, and documentation. DocuForge AI provides built-in support for generating these files automatically from your documentation.

## Format Specification

The standard LLMs.txt file structure includes:

```
# Project Title

> A concise summary of what the project is and does

Optional more detailed explanation that doesn't fit in the summary.

## Required

- [Key Documentation](path/to/key-docs.md): Description of this important file
- [API Reference](path/to/api-reference.md): API documentation
- [Architecture](path/to/architecture.md): System architecture overview

## Optional

- [Additional Information](path/to/additional-info.md): Less critical documentation
- [Examples](path/to/examples.md): Usage examples
- [FAQ](path/to/faq.md): Frequently asked questions
```

## Features of DocuForge AI's LLMs.txt Generator

### Automatic Content Extraction

DocuForge AI analyzes your documentation to:

- Extract the project title from main documentation
- Generate a concise summary of the project
- Identify the most important documentation sections
- Create clean markdown versions of all documentation pages

### Configurable Organization

You can configure:

- Which sections appear in Required vs. Optional categories
- The order of documentation links
- Custom descriptions for each documentation link
- Whether to generate expanded context files

### Expanded Context Files

In addition to the standard llms.txt file, DocuForge AI can generate:

1. **llms-ctx.txt**: Contains key documentation content
2. **llms-ctx-full.txt**: Contains all documentation content

These files provide LLMs with more comprehensive information when needed.

### AI-Optimized Output

The generator uses AI to:

- Create concise, informative summaries
- Select appropriate documentation for required vs. optional sections
- Verify generated files are effective with popular LLM models
- Optimize format for different LLM context windows

## Best Practices

1. Keep the summary concise but informative
2. Include only the most critical documentation in the Required section
3. Organize documentation links logically
4. Provide clear, descriptive labels for documentation links
5. Test your LLMs.txt with different AI assistants
6. Update your LLMs.txt when documentation changes significantly
