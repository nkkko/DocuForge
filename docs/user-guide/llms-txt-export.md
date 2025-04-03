# LLMs.txt Export

## Overview

DocuForge AI provides built-in support for generating LLMs.txt files, a standardized format for making documentation more accessible to large language models (LLMs). This guide walks you through the process of configuring and generating LLMs.txt exports for your projects.

## What is LLMs.txt?

LLMs.txt is a standardized file format that provides information to help language models better understand and interact with your documentation. It serves as an entry point for AI assistants, much like robots.txt serves for search engines.

The format includes:
- Project title and summary
- Required and optional sections of documentation
- Structured links to documentation files

For more details, see the [LLMs.txt Format](../llms-txt-format.md) documentation.

## Generating LLMs.txt Files

### Step 1: Access the LLMs.txt Generator

1. Open your project in DocuForge AI
2. Navigate to the "Export" tab in the main navigation
3. Select "LLMs.txt Generator" from the export options

### Step 2: Configure Your Export

#### Basic Information

- **Project Title**: By default, this uses your project name, but you can customize it
- **Summary**: A concise description of your project (1-2 sentences recommended)
- **Detailed Description**: Optional additional information about your project

#### Required Sections

Select the most important documentation that LLMs should always have access to:

1. Click "Add to Required" to add documentation to this section
2. Drag and drop to reorder documents within the section
3. Edit descriptions to provide context for each document link

#### Optional Sections

Add supplementary documentation that may be useful but isn't essential:

1. Click "Add to Optional" to add documentation to this section
2. Organize and describe these documents as with the Required section

#### Expanded Context Options

- **Generate llms-ctx.txt**: Creates an expanded file with the content of required documents
- **Generate llms-ctx-full.txt**: Creates a comprehensive file with all documentation content

### Step 3: Preview and Test

1. Click "Preview" to see how your generated files will look
2. Use the "Test with AI" feature to verify how well an AI assistant understands your export
3. Make adjustments based on the results

### Step 4: Export

1. Click "Export" when you're satisfied with the configuration
2. Choose where to save the generated files:
   - Project root directory (recommended)
   - Custom location
   - Add to documentation deployment

## Best Practices

### Content Selection

- Include architecture overviews and key concepts in the Required section
- Place detailed API references and examples in the Optional section
- Keep the Required section focused on the most important information

### Descriptions

- Write clear, concise descriptions for each documentation link
- Focus on what information the document contains, not just its title
- Use consistent terminology throughout descriptions

### Testing

- Test your LLMs.txt with different AI assistants to ensure clarity
- Ask the AI questions about your project to verify understanding
- Iterate on your export configuration based on test results

### Maintenance

- Update your LLMs.txt when significant changes occur in your documentation
- Consider regenerating when adding new major features or components
- Keep your project summary up to date

## Advanced Configuration

### Custom Templates

DocuForge AI allows you to create custom templates for LLMs.txt generation:

1. Navigate to Settings > LLMs.txt Templates
2. Click "Create Template"
3. Configure default settings for different project types
4. Apply templates when generating new exports

### Programmatic Generation

For automated workflows, you can use the [LLMs Export API](../api/llms-export.md) to generate exports programmatically.

### Integration with CI/CD

Automatically generate and deploy LLMs.txt files as part of your CI/CD pipeline:

1. Configure webhook integration in your project settings
2. Set up triggers for documentation changes
3. Add deployment steps to your pipeline

See the [CI/CD Integration](./ci-cd-integration.md) guide for detailed instructions.
