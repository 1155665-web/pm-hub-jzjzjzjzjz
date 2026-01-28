# Visual Studio Code Setup Guide for Product Managers

## Overview

Visual Studio Code (VSCode) is a lightweight but powerful code editor that can help product managers work more efficiently with development teams and technical documentation.

## Installation

1. Download VSCode from [code.visualstudio.com](https://code.visualstudio.com/)
2. Install for your operating system (Windows, macOS, or Linux)
3. Launch VSCode

## Essential Extensions for Product Managers

### Documentation & Markdown
- **Markdown All in One**: Enhanced markdown editing
  - Command: `Ctrl+Shift+P` → "Extensions: Install Extensions" → Search "Markdown All in One"
- **Markdown Preview Enhanced**: Better preview for markdown files
- **markdownlint**: Ensure consistent markdown formatting

### Project Management
- **Todo Tree**: Track TODO items across your documentation
- **Project Manager**: Switch between different product projects easily
- **GitLens**: Understand code history and changes

### Collaboration
- **Live Share**: Collaborate in real-time with team members
- **CodeStream**: Review code and discuss with developers
- **GitHub Pull Requests**: Review and comment on PRs directly

### Visualization
- **Draw.io Integration**: Create diagrams and flowcharts
- **PlantUML**: Generate UML diagrams from text
- **Mermaid Preview**: Create flowcharts and diagrams in markdown

## Workspace Setup

### 1. Create a Product Workspace

```
product-management/
├── roadmaps/
├── user-stories/
├── sprint-docs/
├── meeting-notes/
└── decisions/
```

### 2. Configure Settings

Add to your `settings.json` (File → Preferences → Settings → Open Settings JSON):

```json
{
  "markdown.preview.fontSize": 14,
  "markdown.preview.lineHeight": 1.6,
  "editor.wordWrap": "on",
  "files.autoSave": "afterDelay",
  "files.autoSaveDelay": 1000,
  "explorer.confirmDelete": false,
  "workbench.startupEditor": "welcomePage"
}
```

## Useful Keyboard Shortcuts

| Action | Windows/Linux | macOS |
|--------|--------------|-------|
| Command Palette | `Ctrl+Shift+P` | `Cmd+Shift+P` |
| Quick Open File | `Ctrl+P` | `Cmd+P` |
| Toggle Sidebar | `Ctrl+B` | `Cmd+B` |
| Search in Files | `Ctrl+Shift+F` | `Cmd+Shift+F` |
| Toggle Markdown Preview | `Ctrl+Shift+V` | `Cmd+Shift+V` |
| Open Terminal | `Ctrl+\`` | `Cmd+\`` |

## Working with Git

### Setup Git in VSCode

1. Install Git on your system
2. Open Source Control panel (icon on left sidebar)
3. Initialize repository or clone existing one
4. Stage, commit, and push changes directly from VSCode

### Common Git Operations

- **View Changes**: Click Source Control icon
- **Stage Files**: Click `+` next to changed files
- **Commit**: Enter message and click ✓
- **Push**: Click `...` → Push
- **Pull**: Click `...` → Pull

## Tips for Product Managers

### 1. Organize Documentation
- Keep all product docs in a single workspace
- Use folders to separate different types of documents
- Name files consistently (e.g., `2024-Q1-roadmap.md`)

### 2. Markdown for Everything
- Use markdown for all documentation
- Easy to version control with Git
- Can be viewed on GitHub/GitLab without special tools
- Can be converted to other formats if needed

### 3. Integrate with Development Team
- Review code changes with developers
- Understand technical implementation
- Comment on pull requests directly

### 4. Track Tasks
- Use TODO comments in your documentation
- Install Todo Tree extension to see all tasks
- Keep action items visible

### 5. Create Templates
- Create snippet templates for common documents
- Use File → Preferences → User Snippets
- Save time on repetitive documentation

## Example Workflow

1. **Morning**: Open VSCode workspace for current sprint
2. **Review**: Check Git changes from overnight commits
3. **Document**: Update user stories in markdown files
4. **Collaborate**: Join Live Share session for spec review
5. **Track**: Update TODO items based on standup
6. **Version**: Commit and push documentation changes
7. **Review**: Comment on pull requests from development team

## Resources

- [VSCode Documentation](https://code.visualstudio.com/docs)
- [Markdown Guide](https://www.markdownguide.org/)
- [Git Documentation](https://git-scm.com/doc)
