# Document Editor

## Overview

The DocuForge AI Document Editor is a powerful rich text editor that enables you to create and edit documentation with ease. It combines the simplicity of markdown with the richness of visual editing, all while maintaining the structure necessary for documentation-first development.

## Interface Overview

![Document Editor Interface](../assets/images/editor-interface.png)

The editor interface consists of:

1. **Main Toolbar**: Access to formatting, insertion, and AI assistance tools
2. **Side Panel**: Navigation, structure view, and document properties
3. **Editing Area**: The main content editing space
4. **Status Bar**: Document metadata, word count, and saving status
5. **Preview Tab**: Real-time preview of rendered documentation

## Basic Editing

### Text Formatting

The editor supports standard formatting options:

- **Bold**: Use the B button or `Ctrl+B` (`Cmd+B` on Mac)
- **Italic**: Use the I button or `Ctrl+I` (`Cmd+I` on Mac)
- **Underline**: Use the U button or `Ctrl+U` (`Cmd+U` on Mac)
- **Strikethrough**: Use the S button or `Alt+Shift+5`
- **Highlight**: Use the marker button or `Ctrl+Shift+H`

### Headings

Create document structure with headings:

1. Select text or place cursor at the beginning of a line
2. Click the heading dropdown in the toolbar
3. Select heading level (H1-H6)

Alternatively, use markdown syntax:
```
# H1 Heading
## H2 Heading
### H3 Heading
```

### Lists

Create ordered and unordered lists:

- Click the bullet list or numbered list button in the toolbar
- Use `*` or `-` for bullet points in markdown
- Use `1.` for numbered lists in markdown

### Links

Insert links to other documents or external resources:

1. Select text to link
2. Click the link button or press `Ctrl+K` (`Cmd+K` on Mac)
3. Enter the URL or select an internal document
4. Optionally add a title attribute

## Advanced Features

### Code Blocks

Insert and edit code with syntax highlighting:

1. Click the code block button in the toolbar
2. Select the programming language
3. Enter your code

Code blocks support:
- Syntax highlighting for over 100 languages
- Line numbers
- Copy-to-clipboard functionality
- Expandable/collapsible display

### Tables

Create structured data with tables:

1. Click the table button in the toolbar
2. Select dimensions or use the table builder
3. Edit cells, rows, and columns using the context menu

Table features include:
- Column alignment (left, center, right)
- Row and column insertion/deletion
- Cell merging
- Header row/column styling

### Images

Add images to your documentation:

1. Click the image button in the toolbar
2. Upload an image or enter an image URL
3. Add alt text and optional caption
4. Resize and align as needed

### Diagrams

Create diagrams directly in your documentation:

1. Click the diagram button in the toolbar
2. Select diagram type (flowchart, sequence, etc.)
3. Use the diagram editor to create your visualization
4. Save and insert into the document

## AI Assistance

### Writing Suggestions

The editor provides real-time AI suggestions as you write:

1. Enable writing suggestions in the AI menu
2. Watch for suggestion indicators in the text
3. Accept suggestions with `Tab` or reject with `Esc`

### Content Generation

Generate content with AI assistance:

1. Place cursor where you want to insert content
2. Click the "Generate" button in the AI section of the toolbar
3. Describe what you want to generate
4. Review and edit the generated content

### Document Analysis

Use AI to analyze and improve your documentation:

1. Click the "Analyze" button in the AI section
2. Select analysis type (clarity, completeness, etc.)
3. Review suggestions and apply as needed

## Collaboration

### Comments

Add comments to discuss specific parts of documentation:

1. Select text or place cursor at desired location
2. Click the comment button or press `Ctrl+Alt+M`
3. Enter your comment
4. Reply to, resolve, or delete comments as needed

### Change Tracking

Track changes to documentation:

1. Enable change tracking in the View menu
2. View additions, deletions, and modifications
3. Accept or reject changes individually or in bulk

### Real-time Collaboration

Work simultaneously with team members:

1. Share the document link with collaborators
2. See who is currently editing the document
3. View cursors and selections of other users
4. Use the chat panel for discussion

## Version Control

### Automatic Saving

The editor automatically saves your work:

- Changes are saved every 30 seconds
- Manual save with `Ctrl+S` (`Cmd+S` on Mac)
- Save status is shown in the status bar

### Version History

Access previous versions of your documentation:

1. Click the "History" button in the toolbar
2. View list of previous versions with timestamps
3. Compare versions side by side
4. Restore previous versions if needed

### Git Integration

Changes are automatically committed to Git:

1. Every save creates a commit in the background
2. Add commit message in the status bar before saving
3. View commit history in the History panel
4. Create branches and merge changes

## Markdown Mode

Toggle between rich text and markdown editing:

1. Click the "Markdown" button in the toolbar
2. Edit directly in markdown syntax
3. Switch back to rich text mode when finished

Markdown mode features:
- Syntax highlighting
- Live preview
- Keyboard shortcuts
- Auto-completion

## Shortcuts and Efficiency Tips

### Keyboard Shortcuts

Speed up your workflow with these common shortcuts:

| Action | Windows/Linux | Mac |
|--------|--------------|-----|
| Bold | `Ctrl+B` | `Cmd+B` |
| Italic | `Ctrl+I` | `Cmd+I` |
| Link | `Ctrl+K` | `Cmd+K` |
| Save | `Ctrl+S` | `Cmd+S` |
| Undo | `Ctrl+Z` | `Cmd+Z` |
| Redo | `Ctrl+Y` | `Cmd+Shift+Z` |
| Find | `Ctrl+F` | `Cmd+F` |
| Replace | `Ctrl+H` | `Cmd+H` |
| Comment | `Ctrl+Alt+M` | `Cmd+Option+M` |

### Snippets

Use snippets to quickly insert common patterns:

1. Type `/` to open the snippet menu
2. Select or search for a snippet
3. Press `Enter` to insert

Custom snippets can be created in the Settings menu.

### Templates

Start from a template for common documentation types:

1. Click "New from Template" in the File menu
2. Select a template (API Reference, User Guide, etc.)
3. Customize the template for your needs

## Export and Integration

### Export Formats

Export your documentation to various formats:

1. Click the "Export" button in the File menu
2. Select export format:
   - Markdown
   - HTML
   - PDF
   - Word
   - LLMs.txt
3. Configure export options
4. Download or save to project

### Integration with Visual Canvas

Your document automatically appears in the Visual Canvas:

1. Document title becomes a node in the canvas
2. Document headings create a hierarchy
3. Links between documents create edges in the canvas

## Customization

### Editor Preferences

Customize the editor to fit your workflow:

1. Click the "Settings" button in the toolbar
2. Adjust preferences:
   - Theme (light/dark/custom)
   - Font family and size
   - Line spacing
   - Auto-save interval
   - Spell check options
   - AI assistance level

### Toolbar Customization

Personalize the toolbar with your most-used tools:

1. Click the toolbar customization button (gear icon)
2. Drag and drop tools to rearrange
3. Add or remove tools as needed
4. Save your custom configuration

## Troubleshooting

### Recovering Unsaved Changes

If you encounter an issue before saving:

1. Reopen the document
2. Click the "Recover Unsaved Changes" notification
3. Select from available recovery points

### Connection Issues

If you lose connection during editing:

1. The editor will switch to offline mode
2. Continue editing locally
3. Changes will sync when connection is restored

### Support and Feedback

Get help with the editor:

1. Click the "Help" button in the toolbar
2. Access documentation and tutorials
3. Report issues or suggest improvements
4. Contact support for assistance