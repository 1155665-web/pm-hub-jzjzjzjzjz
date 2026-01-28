# IntelliJ IDEA Guide for Product Managers

## Overview

IntelliJ IDEA is a powerful IDE primarily used by Java developers, but it offers valuable features for product managers who need to understand and collaborate on codebases.

## Why IntelliJ for Product Managers?

- **Deep Code Understanding**: Navigate complex codebases easily
- **Built-in Version Control**: Integrated Git support
- **Code Review Tools**: Review changes with context
- **Database Tools**: Understand data models directly
- **Documentation Support**: Write and preview markdown

## Installation

### Community Edition (Free)
1. Visit [jetbrains.com/idea/download](https://www.jetbrains.com/idea/download/)
2. Download Community Edition
3. Install for your operating system
4. Launch IntelliJ IDEA

### Ultimate Edition (Paid)
- Includes additional features like database tools, HTTP client, and more
- 30-day free trial available
- Consider if working heavily with databases or web frameworks

## Initial Setup

### 1. Install Plugins

Navigate to: File → Settings → Plugins (or `Ctrl+Alt+S`)

Essential plugins for PMs:
- **Markdown**: Enhanced markdown editing and preview
- **PlantUML Integration**: Create UML diagrams
- **GitToolBox**: Enhanced Git information
- **CSV Plugin**: View and edit CSV files (useful for data analysis)
- **Database Navigator**: Database exploration (Ultimate has this built-in)

### 2. Configure Settings

**Editor Settings:**
```
File → Settings → Editor → General
- Enable "Show line numbers"
- Enable "Show whitespace"
```

**Version Control:**
```
File → Settings → Version Control
- Enable "Show commit timestamp in blame"
- Enable "Highlight modified files in Project tree"
```

## Understanding the Interface

### Main Components

1. **Project View** (Left): File tree of the project
2. **Editor** (Center): Code and document editing
3. **Tool Windows** (Bottom/Sides): Version control, terminal, database, etc.
4. **Navigation Bar** (Top): Quick navigation through project structure

## Essential Features for Product Managers

### 1. Navigate the Codebase

**Find Files:**
- `Ctrl+Shift+N` (Win/Linux) or `Cmd+Shift+O` (Mac): Find any file
- `Ctrl+N` (Win/Linux) or `Cmd+O` (Mac): Find any class

**Search in Project:**
- `Ctrl+Shift+F` (Win/Linux) or `Cmd+Shift+F` (Mac): Find in files
- Useful for finding where features are implemented

**Go to Definition:**
- `Ctrl+B` or `Ctrl+Click`: Jump to where something is defined
- Understand how features connect

### 2. Version Control Integration

**View Changes:**
- `Alt+9`: Open Version Control tool window
- See all recent commits and changes
- Compare different versions

**Blame/Annotate:**
- Right-click in editor → Git → Annotate with Git Blame
- See who changed each line and when

**Local History:**
- Right-click file → Local History → Show History
- IntelliJ keeps local history even if not committed to Git

### 3. Code Review

**Review Pull Requests:**
- VCS → Git → Pull Requests
- View and comment on PRs directly in IDE
- Understand full context of changes

**Compare Versions:**
- Right-click file → Git → Compare with...
- See exactly what changed between versions

### 4. Database Tools (Ultimate Edition)

**Connect to Database:**
- View → Tool Windows → Database
- Add data source (PostgreSQL, MySQL, etc.)
- Explore tables and relationships

**Understand Data Models:**
- View table structures
- See relationships between tables
- Run queries to understand data

## Useful Shortcuts for PMs

| Action | Windows/Linux | macOS |
|--------|--------------|-------|
| Search Everywhere | `Double Shift` | `Double Shift` |
| Find File | `Ctrl+Shift+N` | `Cmd+Shift+O` |
| Find in Files | `Ctrl+Shift+F` | `Cmd+Shift+F` |
| Recent Files | `Ctrl+E` | `Cmd+E` |
| Go to Definition | `Ctrl+B` | `Cmd+B` |
| Show Usages | `Ctrl+Alt+F7` | `Cmd+Alt+F7` |
| Terminal | `Alt+F12` | `Option+F12` |
| VCS Operations | `Alt+\`` | `Control+V` |

## PM Workflows in IntelliJ

### 1. Feature Specification Review

```
1. Open project in IntelliJ
2. Find relevant code files (Ctrl+Shift+N)
3. Read implementation
4. Check Git history for context (Alt+9)
5. Add comments or questions
6. Discuss with developers
```

### 2. Bug Investigation

```
1. Search for error message (Ctrl+Shift+F)
2. Navigate to code location
3. Check recent changes (Git → Annotate)
4. Review related files
5. Document findings for developers
```

### 3. Technical Specification

```
1. Navigate codebase to understand current implementation
2. Identify affected files and classes
3. Create markdown spec in project
4. Reference specific files and line numbers
5. Commit spec to version control
```

### 4. Data Analysis

```
1. Connect to database (Database tool window)
2. Explore table structures
3. Run queries to understand data
4. Export results for analysis
5. Document data requirements
```

## Creating Product Documentation

### Markdown Files

IntelliJ has excellent markdown support:
- Create `.md` files in your project
- Live preview available (split editor)
- Support for tables, code blocks, links
- Can be versioned with code

### Linking to Code

Reference specific files and lines in your documentation:
```markdown
See implementation in `UserService.java:45-60`
```

## Integration with Development Team

### 1. Code Reviews
- Comment directly on code
- Understand implementation details
- Provide informed feedback

### 2. Sprint Planning
- Estimate complexity by reviewing code
- Identify dependencies between features
- Understand technical constraints

### 3. Technical Discussions
- Navigate code during discussions
- Reference specific implementations
- Make informed product decisions

## Tips and Best Practices

### For Non-Technical PMs
1. **Don't be intimidated**: You don't need to understand every line
2. **Focus on structure**: Understand file organization and relationships
3. **Use search**: Find specific features or terms quickly
4. **Ask developers**: They can explain complex parts
5. **Learn gradually**: Pick up more understanding over time

### For Technical PMs
1. **Deep dive**: Use IntelliJ's navigation to fully understand implementations
2. **Review thoroughly**: Check edge cases and error handling
3. **Suggest improvements**: Provide technical feedback on PRs
4. **Maintain perspective**: Remember you're a PM, not a developer

### General Tips
- Keep IntelliJ open during sprint planning
- Reference actual code when writing specs
- Use local history as a safety net
- Explore the codebase regularly to stay current

## Resources

- [IntelliJ IDEA Documentation](https://www.jetbrains.com/idea/documentation/)
- [IntelliJ IDEA Tips & Tricks](https://www.jetbrains.com/idea/guide/)
- [Git in IntelliJ](https://www.jetbrains.com/help/idea/version-control-integration.html)
