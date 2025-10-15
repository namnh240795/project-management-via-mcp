# GitHub Copilot Instructions - Project Management via MCP

## 🎯 Project Overview & Context

This repository contains **project-management-via-mcp**, a comprehensive project management system that integrates GitHub Projects with Model Context Protocol (MCP). When interacting with this project, always maintain awareness of the following context:

### Repository Information

- **Repository**: `namnh240795/project-management-via-mcp`
- **Owner**: namnh240795 (Nam Nguyễn)
- **Primary Branch**: main
- **GitHub Project**: Project #6 (https://github.com/users/namnh240795/projects/6)
- **Project Status**: Active development, Phase 1 in progress

## 📋 Current Project Fields

The following fields are configured in GitHub Project #6:

1. **Title**
2. **Assignees**
3. **Status** (options: Todo, In Progress, Done)
4. **Labels**
5. **Linked pull requests**
6. **Milestone**
7. **Repository**
8. **Reviewers**
9. **Parent issue**
10. **Sub-issues progress**
11. **Start Date**
12. **Target Date**
13. **Iteration**

These fields are used for comprehensive project and workflow management.

**Note:**  
 When adding or updating the **Start Date** and **Target Date** fields for issues in GitHub Project #6, use the mcp_github-projec_update_project_item` API.

- The field ID for **Start Date** is `230314687`.
- The field ID for **Target Date** is `230314819`.
- The `item_id` should be the project item ID of the issue.
- The value should be in `YYYY-MM-DD` format.
