# Visual Canvas

## Overview

The Visual Canvas is a powerful feature of DocuForge AI that allows you to visualize, organize, and navigate your documentation structure. It provides an intuitive, graph-based interface for understanding relationships between documents and managing the overall architecture of your documentation.

## Interface Elements

![Visual Canvas Interface](../assets/images/canvas-interface.png)

The Visual Canvas interface consists of:

1. **Main Canvas Area**: Interactive graph visualization of documents
2. **Toolbar**: Tools for manipulating the canvas
3. **Mini-map**: Overview of the entire canvas with viewport indicator
4. **Properties Panel**: Details and settings for selected elements
5. **Filters Panel**: Options to filter what's displayed on the canvas

## Basic Navigation

### Viewing the Canvas

Navigate around the canvas using these techniques:

- **Pan**: Click and drag on empty space
- **Zoom**: Use mouse wheel or pinch gesture on trackpad
- **Reset View**: Double-click on empty space
- **Fit to View**: Press the "Fit" button in the toolbar

### Selection

Interact with elements on the canvas:

- **Select Node**: Click on a document node
- **Select Multiple**: Hold `Shift` while clicking or drag a selection box
- **Select All**: Press `Ctrl+A` (`Cmd+A` on Mac)
- **Deselect**: Click on empty space

## Document Nodes

### Node Types

The canvas displays different types of nodes:

- **Document Nodes**: Represent individual documentation files
- **Section Nodes**: Represent major sections or folders
- **External Nodes**: Represent external resources or links
- **Group Nodes**: Contain multiple related nodes

Each node type has a distinct visual appearance for easy identification.

### Node Properties

Nodes display key information about documents:

- **Title**: Document title (displayed on node)
- **Status**: Implementation status (color-coded)
- **Owner**: Assigned owner (optional avatar)
- **Type**: Document type (icon indicator)
- **Priority**: Importance level (border style)

### Interacting with Nodes

Perform actions on document nodes:

- **Open Document**: Double-click a node
- **Quick Preview**: Hover over a node (shows tooltip with summary)
- **Move Node**: Drag to new position
- **Resize Node**: Drag handles when selected
- **Access Menu**: Right-click for context menu

## Connections

### Edge Types

Connections between nodes are represented by edges:

- **Reference Edge**: Document references another document
- **Dependency Edge**: Document depends on another document
- **Sequence Edge**: Documents that should be read in sequence
- **Inheritance Edge**: Document extends or inherits from another

Each edge type has a distinct visual style (color, line pattern, thickness).

### Creating Connections

Connect documents to show relationships:

1. Select a source node
2. Click the "Connect" button in the toolbar
3. Click on a target node
4. Select connection type from the popup menu

Alternatively, start a connection by dragging from a node's connection point.

### Editing Connections

Modify existing connections:

- **Change Type**: Select edge and choose new type from properties panel
- **Add Label**: Double-click on edge to add description
- **Adjust Path**: Drag edge control points
- **Delete**: Select edge and press `Delete` or use context menu

## Organizing Documentation

### Manual Arrangement

Organize nodes to reflect logical structure:

1. Select nodes to arrange
2. Drag to position them manually
3. Use alignment tools in the toolbar for precise arrangement

### Auto Layout

Apply automatic layouts to organize your canvas:

1. Select nodes to include (or all nodes)
2. Click the "Layout" button in the toolbar
3. Choose a layout algorithm:
   - Hierarchical (top-down or left-right)
   - Force-directed (natural clustering)
   - Circular (radial arrangement)
   - Grid (ordered grid pattern)
4. Adjust layout options if needed
5. Apply the layout

### Grouping

Create logical groups of related documents:

1. Select nodes to group
2. Click the "Group" button or press `Ctrl+G` (`Cmd+G` on Mac)
3. Name the group
4. Customize group appearance (color, icon)

Groups can be collapsed/expanded to simplify complex diagrams.

## Canvas Features

### Filtering

Focus on specific aspects of your documentation:

1. Open the Filters panel
2. Filter by attributes:
   - Document type
   - Status
   - Owner
   - Tags
   - Modified date
3. Save filter presets for common views

### Search

Locate specific documents on the canvas:

1. Click the search icon or press `Ctrl+F` (`Cmd+F` on Mac)
2. Enter search terms
3. Review matching results
4. Click a result to highlight and focus on that node

### Tags and Metadata

Use tags to categorize and filter documents:

1. Select a node
2. Add tags in the Properties panel
3. Create custom metadata fields as needed
4. Use the Filters panel to filter by tags/metadata

## Advanced Features

### Presentation Mode

Create guided tours of your documentation:

1. Select nodes in the sequence you want to present
2. Click "Create Presentation" in the View menu
3. Add notes for each step
4. Save the presentation
5. Use the presentation controls to navigate through steps

### Versioning and History

Track changes to your documentation structure:

1. Access canvas history from the History menu
2. View snapshots of the canvas at different points in time
3. Compare changes between versions
4. Restore previous arrangements if needed

### Collaboration

Work together on the same canvas:

1. Share the canvas with team members
2. See real-time updates as others modify the canvas
3. Use the chat panel for discussions about structure
4. Leave notes on the canvas for team members

### Export and Sharing

Share your documentation structure:

1. Click the "Export" button in the toolbar
2. Choose export format:
   - Image (PNG, JPEG, SVG)
   - PDF
   - Interactive HTML
   - JSON data
3. Configure export options (size, quality, included elements)
4. Download or share directly

## Integration with Editor

### Auto-updating Connections

The canvas automatically reflects document relationships:

- When you add a link in the Document Editor, a connection appears on the canvas
- When you restructure documents, the canvas updates to show new relationships
- When you create new documents, they appear as new nodes

### Visual Navigation

Use the canvas as a navigation tool for your documentation:

1. Open the Visual Canvas alongside the Document Editor
2. Click nodes to open the corresponding documents
3. The currently open document is highlighted on the canvas

## Customization

### Canvas Themes

Personalize the appearance of your canvas:

1. Access Canvas Settings from the toolbar
2. Select from predefined themes or create a custom theme
3. Customize colors, fonts, node styles, and background
4. Save custom themes for reuse

### Layout Preferences

Set default layout preferences:

1. Access Canvas Settings
2. Configure default layout algorithm
3. Set spacing, orientation, and other layout parameters
4. Define default node appearance for different document types

## Best Practices

### Structure Planning

Effectively plan your documentation structure:

1. Start with high-level section nodes
2. Add key document nodes for main topics
3. Establish primary relationships between documents
4. Gradually add detail as your documentation grows

### Visual Communication

Use visual elements to communicate document status and relationships:

- Use consistent color coding for document status
- Group related documents visually
- Use edge types consistently to show relationship types
- Add labels to clarify complex relationships

### Canvas Organization

Keep your canvas manageable and informative:

- Use groups to organize related content
- Create multiple canvases for different aspects of your documentation
- Use filters to create focused views
- Regularly clean up and reorganize as your documentation evolves

## Troubleshooting

### Performance Issues

For large documentation sets:

1. Use filtering to reduce visible elements
2. Collapse groups when not needed
3. Consider splitting very large structures into multiple canvases
4. Adjust rendering quality in settings for better performance

### Common Problems

Solutions to frequent issues:

- **Node not appearing**: Check filters, refresh the canvas
- **Can't create connection**: Verify that the connection type is allowed between those node types
- **Layout not working well**: Try different layout algorithms or adjust parameters
- **Canvas becoming cluttered**: Use groups and filters to organize content