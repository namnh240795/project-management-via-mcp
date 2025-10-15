# GitHub Copilot Instructions

## Project Context

This is a project management system that uses Model Context Protocol (MCP) to integrate with GitHub services including issues, labels, projects, and repositories.

<!-- ## Working with Wiki

When the user mentions "wiki" or "documentation":

- Always reference and work with files in the `/wiki` directory of this repository
- The wiki contains the Software Requirements Specification (SRS) and project documentation
- When updating or creating wiki content, maintain the existing structure and format
- Wiki files are in Markdown format and should follow documentation best practices -->

## Working with GitHub Projects

When the user mentions "project" or "GitHub project":

- Work with the GitHub Project board attached to the `namnh240795/project-management-via-mcp` repository
- Use the MCP servers configured in `.vscode/mcp.json` to interact with:
  - GitHub Issues (`github-issues`)
  - GitHub Labels (`github-labels`)
  - GitHub Projects (`github-projects`)
  - GitHub Repositories (`github-repos`)
- Understand that "project" refers to the GitHub Project management tool, not the entire codebase

## MCP Integration

This project uses the following MCP servers:

- **github**: General GitHub API access
- **github-issues**: For managing issues
- **github-labels**: For managing labels
- **github-projects**: For managing project boards
- **github-repos**: For repository operations

When working with project management tasks, leverage these MCP integrations to interact with GitHub resources.

## Best Practices

1. **Wiki Updates**: Always check existing wiki content before creating new pages to avoid duplication
2. **Project Management**: When creating or updating issues, ensure they follow the project's labeling and organization standards
3. **Documentation**: Keep wiki documentation synchronized with actual project features and requirements
4. **Version Control**: All wiki changes should be committed to the repository for version tracking
