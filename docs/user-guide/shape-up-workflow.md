# Shape Up Workflow in DocuForge AI

## Overview

DocuForge AI integrates the Shape Up methodology from Basecamp/37signals directly into its documentation-first workflow. This guide explains how DocuForge implements the Shape Up concepts and how to use these features to manage your product development process.

## Key Shape Up Concepts in DocuForge

### 1. Shaping Through Documentation

In DocuForge AI, the documentation-first approach serves as the foundation of the shaping process:

- **Appetite Setting**: Define the scope and constraints of work upfront
- **Solution Boundaries**: Outline what's in and out of scope
- **Risk Reduction**: Identify and address risks early in documentation
- **Feasibility Checks**: Validate technical approaches through documentation

### 2. Six-Week Cycles

DocuForge AI organizes work into six-week cycles:

- **Cycle Planning**: Define and organize documentation for upcoming work
- **Cycle View**: Visual representation of current cycle's documentation status
- **Progress Tracking**: Monitor documentation and implementation progress
- **Cool-down Period**: Dedicated time for refining documentation between cycles

### 3. Betting Table

The betting table concept is implemented as a structured decision-making interface:

- **Pitch Repository**: Collect and evaluate documentation pitches
- **Betting Meeting Support**: Tools for reviewing and selecting pitches
- **Commitment Tracking**: Document decisions and assigned teams
- **Resources Allocation**: Track team assignments and dependencies

## Implementing Shape Up with DocuForge

### Creating Pitches as Documentation

1. Navigate to the **Pitches** section
2. Click **New Pitch**
3. Use the pitch template which includes:
   - Problem statement
   - Appetite (small batch: 2 weeks, big batch: 6 weeks)
   - Solution boundaries
   - Rabbit holes to avoid
   - No-gos
   - Visual mockups or diagrams

Each pitch is a complete documentation package that serves as both the shaping artifact and the beginning of project documentation.

### Running the Betting Table

1. Access the **Betting Table** view at the end of a cycle
2. Review available pitches with their full documentation
3. Use the built-in voting and commenting tools
4. Select pitches to be worked on in the next cycle
5. Assign teams to selected pitches
6. Automatically generate cycle documentation

### Working in Cycles

Once bets are placed, DocuForge helps teams work without interruption:

1. Teams access their assigned documentation through the **Current Cycle** dashboard
2. Documentation evolves as the team makes progress
3. Track implementation status against documentation specifications
4. Use the built-in **Hill Chart** view to monitor progress:
   - Uphill: Figuring things out
   - Downhill: Execution with known solutions

The visual canvas displays work in a hill-chart format, showing both documentation and implementation progress.

## Shape Up Document Templates

DocuForge AI provides specialized templates aligned with Shape Up methodology:

### Pitch Template

```markdown
# [Feature Name] Pitch

## Problem
[Clear description of the problem we're solving]

## Appetite
[Time constraint: Small Batch (2 weeks) or Big Batch (6 weeks)]

## Solution
[The core solution, including wireframes and key flows]

## Boundaries
[What's specifically included and excluded]

## Rabbit Holes
[Potential areas where we could get stuck]

## No-gos
[Things we're explicitly not doing]

## Implementation Notes
[Technical considerations that influence the solution]
```

### Hill Chart Status Template

```markdown
# Hill Chart Status: [Feature Name]

## Current Position
- [ ] Problem Understanding (Uphill)
- [ ] Solution Exploration (Uphill)
- [x] Solution Definition (Top of Hill)
- [ ] Implementation Started (Starting Downhill)
- [ ] Implementation Progress (Downhill)
- [ ] Implementation Complete (Bottom of Hill)

## Uphill Discoveries
[New learnings that have shaped our understanding]

## Downhill Progress
[Clear implementation steps and status]

## Blockers
[Current challenges or dependencies]
```

## Integration with Visual Canvas

DocuForge's Visual Canvas provides specialized views for Shape Up workflows:

1. **Scopes View**: Organizes documentation by team-assigned scopes
2. **Hill Chart View**: Visualizes progress across all scopes
3. **Cycle Timeline**: Shows documentation and implementation status over time
4. **Betting Table View**: Interface for review and selection of pitches

Each view is automatically generated from your documentation structure.

## Integration with LLMs.txt Export

Shape Up documentation can be included in your LLMs.txt exports:

```
# Project Name

> Project summary

## Required

- [Pitches](pitches/README.md): Current and past project pitches
- [Current Cycle](cycles/current.md): Active work in progress
- [Shape Up Process](process.md): Our adaptation of Shape Up

## Optional

- [Previous Cycles](cycles/): History of completed work
- [Betting Table Records](betting/): Past betting decisions
```

This ensures AI tools can understand your Shape Up process and assist with both shaping work and implementation.

## Best Practices

### Documentation as Shaping

- Create documentation with the right level of abstraction
- Focus on boundaries and constraints over detailed specifications
- Include both the "appetite" and the "solution" in documentation
- Use diagrams and wireframes to communicate visually
- Document rabbit holes and no-gos explicitly

### Managing Cycles

- Keep cycle documentation separate from general documentation
- Update documentation as work progresses through the hill
- Document discovered scope during implementation
- Use the cool-down period to refine and organize documentation
- Maintain a clean boundary between cycles

### Effective Betting

- Ensure all pitched documentation is shaped properly before betting
- Document betting decisions and rationales
- Link pitches to strategic documentation
- Use the cool-down period to prepare pitches for the next cycle
- Document explicitly what was not selected and why

## Advanced Features

### Automatic Cycle Reports

Generate end-of-cycle reports that include:
- Documentation changes during the cycle
- Implementation status against documentation
- Discovered scope and additional documentation
- Recommendations for future improvements

### Pitch Refinement with AI

Use DocuForge AI features to improve pitch documentation:
1. Select a draft pitch
2. Click "Shape with AI"
3. The AI will analyze for:
   - Missing boundaries
   - Potential rabbit holes
   - Unclear scope
   - Implementation risks
4. Review and incorporate AI suggestions

### Hill Chart Forecasting

DocuForge AI can analyze documentation completeness and implementation progress to forecast delivery:
1. Access the "Forecast" tab in the cycle view
2. Review AI-generated predictions based on documentation quality and implementation status
3. Identify potential risks based on documentation gaps

## Conclusion

By integrating Shape Up methodology directly into DocuForge AI's documentation-first approach, teams can:

1. Use documentation as the primary shaping artifact
2. Manage work in focused six-week cycles
3. Make better betting decisions with complete information
4. Track progress visually through hill charts
5. Maintain a clear record of decisions and rationales

This integration ensures that documentation remains the single source of truth throughout the entire product development lifecycle, from initial shaping to final implementation.