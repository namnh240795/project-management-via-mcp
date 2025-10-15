# project-management-via-mcp

## Overview

This repository provides a comprehensive project management system that integrates GitHub Projects with the Model Context Protocol (MCP). The goal is to streamline project tracking, issue management, and workflow automation by leveraging both GitHub's project management features and the extensibility of MCP.

## How It Works

- **GitHub Projects Integration**:  
  The repository is connected to a GitHub Project (Project #6), which is used to manage issues, tasks, and workflows. Each issue or pull request can be tracked as a project item with custom fields such as Status, Type, Assignees, Start Date, Target Date, and more.

- **Model Context Protocol (MCP)**:  
  MCP acts as a bridge between GitHub and external tools or automations. It enables programmatic updates to project fields, synchronization of issue metadata, and advanced workflow automation.

- **Custom Project Fields**:  
  The project uses custom fields for detailed tracking:

  - Status (e.g., Todo, In Progress, Dev Done, etc.)
  - Type (Phase, Epic, User Story, Backend Task, Frontend Task, Bug)
  - Start Date and Target Date (managed via MCP API)
  - Assignees, Labels, Milestone, Reviewers, Sub-issues, and more

- **Automated Updates**:  
  When issues or pull requests are created or updated, MCP can automatically update the corresponding project item fields (such as Start Date and Target Date) using the MCP GitHub Project API.

## Usage

1. **Create or Update Issues**:  
   Add issues or pull requests as usual in GitHub. They will be tracked in the GitHub Project.

2. **Project Field Management**:  
   Use MCP to programmatically update project fields. For example, to set the Start Date or Target Date, use the MCP API with the appropriate field IDs.

3. **Workflow Automation**:  
   Automations can be built on top of MCP to move issues through different statuses, assign users, or update fields based on external triggers.

## Project Field IDs

- **Start Date**: `230314687`
- **Target Date**: `230314819`

To update these fields via MCP, use the `mcp_github-projec_update_project_item` API with the project item ID and the value in `YYYY-MM-DD` format.

## Example MCP API Usage

```json
{
  "item_id": "<project_item_id>",
  "owner": "namnh240795",
  "owner_type": "user",
  "project_number": 6,
  "updated_field": {
    "id": 230314687,
    "value": "2025-10-15"
  }
}
```
