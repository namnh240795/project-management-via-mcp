# GitHub Copilot Instructions - Project Management via MCP

## 🎯 Project Overview & Context

This repository contains **project-management-via-mcp**, a comprehensive project management system that integrates GitHub Projects with Model Context Protocol (MCP). When interacting with this project, always maintain awareness of the following context:

### Repository Information

- **Repository**: `namnh240795/project-management-via-mcp`
- **Owner**: namnh240795 (Nam Nguyễn)
- **Primary Branch**: main
- **GitHub Project**: Project #6 (https://github.com/users/namnh240795/projects/6)

## 📋 Current Project Fields

The following fields are configured in GitHub Project #6:

- Title
- Assignees
- Status (options: Todo, In Progress, Dev Done, Ready On SIT, Testing On SIT, Ready To UAT, Ready On UAT, Testing On UAT, Ready To Production, Ready On Production)
- Labels
- Linked pull requests
- Milestone
- Repository
- Reviewers
- Parent issue
- Sub-issues progress
- Start Date (date)
- Target Date (date)
- Type (options: Phase, Epic, User Story, Backend Task, Frontend Task, Bug)

These fields are used for comprehensive project and workflow management.

**Note:**  
 When adding or updating the **Start Date** and **Target Date** fields for issues in GitHub Project #6, use the mcp_github-projec_update_project_item` API.

- The field ID for **Start Date** is `230314687`.
- The field ID for **Target Date** is `230314819`.
- The `item_id` should be the project item ID of the issue.
- The value should be in `YYYY-MM-DD` format.
