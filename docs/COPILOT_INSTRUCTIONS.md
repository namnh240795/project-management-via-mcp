# 🤖 GitHub Copilot Instructions for Project Management

## 📋 Project Context
This repository contains a project management system that integrates with GitHub Projects via Model Context Protocol (MCP). The project follows a structured 4-phase development approach with comprehensive tracking and automation.

## 🎯 Copilot Automation Guidelines

### Project Structure Understanding
When working with this project, GitHub Copilot should be aware of:

- **Repository**: `namnh240795/project-management-via-mcp`
- **GitHub Project**: Project #6 (https://github.com/users/namnh240795/projects/6)  
- **Development Phases**: 4 structured phases (Foundation → Core → Advanced → Polish)
- **Issue Management**: All issues are linked to the project board
- **Documentation**: Comprehensive docs in `/docs` directory

### 🔄 Automated Task Management

#### Issue Creation Guidelines:
```markdown
When creating new issues, always include:
- Clear, descriptive title following pattern: "Phase X: [Feature/Task Name]"
- Comprehensive body with objectives, deliverables, and acceptance criteria  
- Appropriate labels: phase-X, priority level, feature type
- Milestone assignment if applicable
- Link to parent issues for sub-tasks
```

#### Project Board Integration:
```yaml
Status Management:
  - New issues: Automatically assign to "Todo" status
  - Active work: Move to "In Progress" 
  - Completed work: Move to "Done"
  - Link related PRs automatically

Field Updates:
  - Assignees: Auto-assign based on @mentions or context
  - Labels: Apply phase and priority labels consistently  
  - Milestones: Link to appropriate release milestones
  - Parent/Child: Maintain issue hierarchy
```

### 📊 View-Specific Instructions

#### Main Kanban Board Usage:
- Primary view for daily workflow management
- Keep "In Progress" column focused (max 3-4 items)
- Move completed items to "Done" immediately
- Use for daily standups and progress tracking

#### Timeline/Roadmap View Usage:  
- Long-term planning and milestone visualization
- Update when phase timelines change
- Use for sprint planning and dependency mapping
- Maintain realistic date estimates

#### Priority Matrix Usage:
- Resource allocation and task prioritization  
- High priority items get immediate attention
- Medium priority items scheduled for future sprints
- Review weekly during planning sessions

### 🏷️ Label Management Strategy

#### Phase Labels:
- `phase-1`: Foundation setup tasks
- `phase-2`: Core feature development  
- `phase-3`: Advanced features and analytics
- `phase-4`: Polish, testing, and documentation

#### Priority Labels:
- `high-priority`: Critical path, blocks other work
- `medium-priority`: Important but flexible timing
- `low-priority`: Nice-to-have, future consideration

#### Feature Type Labels:
- `core-features`: Essential functionality
- `advanced-features`: Enhanced capabilities
- `documentation`: Docs, guides, README updates
- `testing`: QA, unit tests, integration tests
- `enhancement`: New feature requests
- `bug`: Issue fixes and corrections

### 🤖 Copilot Automation Workflows

#### 1. Issue Triage Automation:
```yaml
When: New issue created
Actions:
  - Analyze title and body for phase keywords
  - Auto-apply appropriate phase label  
  - Set initial priority based on description
  - Add to project board in "Todo" status
  - Suggest assignee based on expertise area
```

#### 2. PR Integration Automation:
```yaml
When: Pull Request opened
Actions:
  - Link to related issues automatically
  - Move linked issues to "In Progress"  
  - Add appropriate reviewers based on file changes
  - Update project item status
  - Check for documentation requirements
```

#### 3. Completion Automation:
```yaml
When: Issue closed or PR merged
Actions:
  - Move project item to "Done" status
  - Update parent issue progress if applicable
  - Check if milestone completion criteria met
  - Generate completion notifications
  - Update project metrics
```

### 📝 Code Generation Guidelines

#### MCP Integration Code:
```typescript
// When generating MCP-related code, follow these patterns:
class MCPProjectManager {
  // Always include proper error handling
  // Use TypeScript for type safety
  // Follow established naming conventions
  // Include comprehensive JSDoc comments
}
```

#### GitHub API Integration:
```typescript  
// Use official GitHub REST/GraphQL APIs
// Implement proper authentication handling
// Add retry logic for rate limiting
// Cache responses appropriately
```

#### Project Management Features:
```typescript
// Focus on user experience and automation
// Minimize manual intervention required
// Provide clear feedback and status updates
// Support both CLI and UI interactions
```

### 📚 Documentation Requirements

#### Auto-Generated Documentation:
- API documentation from code comments
- README updates when features change
- Changelog entries for significant updates
- Architecture diagrams for complex features

#### Manual Documentation:
- User guides for new features  
- Setup and configuration instructions
- Troubleshooting guides
- Integration examples

### 🔍 Code Review Automation

#### Automated Checks:
```yaml
PR Review Criteria:
  - Code follows project conventions
  - Tests are included for new features
  - Documentation is updated as needed
  - No security vulnerabilities introduced
  - Performance impact is considered
```

#### Review Assignment:
- Route frontend changes to UI specialists
- Route backend changes to API developers
- Route documentation changes to technical writers
- Route critical changes to senior developers

### 📈 Metrics and Reporting

#### Automated Metrics Collection:
```yaml
Track:
  - Issue completion velocity  
  - Phase progression timing
  - Code review turnaround
  - Bug discovery rate
  - Feature usage statistics
```

#### Weekly Reports:
- Progress against roadmap milestones
- Team velocity and capacity
- Blockers and impediments
- Upcoming sprint planning items

### 🚀 Deployment and Release

#### Release Preparation:
```yaml
Pre-Release Checklist:
  - All phase objectives completed
  - Test coverage meets requirements (90%+)
  - Documentation is up to date
  - Security scan passes
  - Performance benchmarks met
```

#### Release Automation:
- Tag creation with semantic versioning
- Changelog generation from commits
- Deployment to staging environment  
- Production deployment after approval
- Post-deployment monitoring

### 🔧 Development Environment

#### Setup Automation:
```bash
# Auto-generate setup scripts for:
npm install           # Dependencies
npm run setup        # Environment configuration  
npm run test         # Validation
npm run dev          # Development server
```

#### Code Quality:
```yaml
Automated Checks:
  - ESLint for code style
  - Prettier for formatting
  - TypeScript for type checking
  - Jest for unit testing
  - Cypress for E2E testing
```

### 💡 AI-Assisted Development

#### Feature Development:
- Suggest optimal implementation patterns
- Generate boilerplate code for common tasks
- Provide security best practices
- Recommend performance optimizations

#### Bug Resolution:
- Analyze error logs and stack traces
- Suggest root cause investigations
- Recommend fix strategies
- Generate regression tests

#### Code Refactoring:
- Identify code smells and technical debt
- Suggest modernization opportunities  
- Recommend architectural improvements
- Generate migration scripts

---

## 🎯 Key Success Metrics

- **Issue Resolution Time**: < 3 days average
- **Phase Completion Rate**: 100% within timeline
- **Code Quality Score**: 90%+ (SonarQube)
- **Test Coverage**: 90%+ for critical paths
- **Documentation Coverage**: 100% for public APIs

## 📞 Emergency Procedures

### Critical Issue Response:
1. Create high-priority issue immediately
2. Assign to project lead  
3. Move to "In Progress" status
4. Notify stakeholders via GitHub notifications
5. Track resolution in dedicated project view

### Deployment Rollback:
1. Trigger automated rollback procedures
2. Create incident tracking issue
3. Coordinate team communication
4. Document lessons learned
5. Update deployment procedures

---

**Last Updated**: October 15, 2025  
**Copilot Version Compatibility**: GitHub Copilot (Latest)  
**Integration Status**: Active