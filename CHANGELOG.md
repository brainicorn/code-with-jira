# Change Log

All notable changes to Code with Jira will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.0] - 2026-01-15

Initial public release of **Code with Jira** - The new standard in Jira/IDE integration.

### Added

#### Core Jira Integration
- OAuth 2.0 authentication with persistent sessions
- Multi-site support for connecting to multiple Jira Cloud instances
- Secure credential storage using VS Code's secret storage API
- Quick site switching between multiple connected Jira instances

#### Work Items Tree View
- Custom JQL queries with full syntax support
- Create, edit, rename, and delete saved JQL queries
- Hierarchical issue display showing parent-child relationships
- Active issue highlighting for currently active work
- Drag and drop re-parenting of issues
- Quick action buttons on tree items for common operations
- Context menu with comprehensive issue actions
- Real-time refresh and update capabilities
- Configurable pagination for large result sets

#### Spaces (Projects) Tree View
- Project-based navigation across all connected sites
- Pin/unpin favorite projects for quick access
- Pre-built quick filters per project (My Open, Recently Updated, Current Sprint)
- Automatic board and backlog link detection
- Create issues directly from project nodes
- Multi-site project management

#### Rich Work Item Editor
- Responsive split-pane layout adapting to viewport size
- Full Atlassian Document Format (ADF) support for rich text editing
- Rich formatting: bold, italic, lists, code blocks, tables, @mentions
- All standard and custom Jira fields supported
- Attachment upload and management
- Issue linking (blocks, relates to, etc.)
- Remote links for external URLs
- Sub-task viewing and management
- Activity stream with comments and history
- Status transitions with transition screen support
- Real-time validation and error handling

#### Start/Stop Work Flow
- One-click start work with comprehensive automation
- Automatic git branch creation with configurable naming templates
- Branch naming variables: `${issueKey}`, `${issueSummary}`, `${issueType}`, `${projectKey}`
- Configurable branch prefixes based on issue type
- Automatic issue status transition to "In Progress"
- Automatic issue assignment to current user
- Optional parent issue transition
- Turbo mode for skipping confirmation dialogs
- Smart branch detection and tracking
- Automatic stop work when branch is deleted (after PR merge)
- Configurable behavior for temporary branch switches
- Optional transition to "Done" when stopping work

#### Time Tracking
- Automatic time tracking while working on issues
- Work session management integrated with start/stop flow
- Automatic work log creation in Jira
- Manual time logging support
- Accurate per-issue time tracking

#### Comment Tags Management
- Automatic workspace scanning for TODO, FIXME, HACK, NOTE, BUG tags
- Configurable custom tag types with color coding
- Multiple view modes: group by tag type or group by file
- Hierarchical file tree with compact folder display option
- Jira issue key detection and linking in tags
- One-click navigation to tag location in source code
- Create Jira issues directly from comment tags
- Issue key automatically added back to comment after creation
- Configurable include/exclude glob patterns
- Respects .gitignore by default
- Real-time file watching and updates
- Multiple scan modes: workspace, open files, or both
- Tag statistics and distribution display

#### JQL Editor
- Intelligent auto-completion for fields, operators, values, and functions
- Context-aware suggestions based on cursor position
- Field value lookup from actual Jira data
- Error highlighting for syntax validation
- Rich data grid for search results
- Sort and filter capabilities
- Click to open issues in full editor
- Inline actions and context menu on results

#### Work Item Creation
- Smart QuickPick for fast issue creation
- Full editor mode for complex issue types
- Automatic escalation from QuickPick to editor when needed
- Create child issues directly from parent
- Pre-fill support from comment tags
- Support for all Jira field types including custom fields
- Attachment upload during creation
- Issue and remote link creation
- Project and issue type validation

#### AI Features (GitHub Copilot Integration)
- Chat participant `@codewithjira` for Jira-aware assistance
- Natural language issue exploration and navigation
- AI-powered planning agent for creating issue hierarchies
- Natural language to Epic → Task → Sub-task breakdown
- Smart issue type selection based on Jira project configuration
- AI-generated labels and descriptions
- Draft review before issue creation
- Start/stop work via chat commands
- Navigate issue hierarchies with AI assistance
- AI-recommended task ordering based on dependencies
- Full suite of Language Model tools for automation
- Non-interactive tool operation for seamless automation
- Context-aware AI with workspace and Jira understanding

#### Help & Feedback
- Integrated help and feedback tree view
- Getting started guide and quick onboarding
- Direct links to documentation
- Streamlined bug reporting flow
- Feature request access via GitHub issues
- Rate extension link to marketplace
- Direct feedback submission mechanism

### Technical
- Built on VS Code Extension API 1.106.0+
- Full Jira Cloud REST API v3 integration
- OAuth 2.0 authentication flow
- Intelligent caching with cache invalidation
- Localization support (l10n ready)
- TypeScript codebase with strict type checking
- Comprehensive error handling and logging

---

## Version History

[Unreleased]: https://github.com/brainicorn/code-with-jira/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/brainicorn/code-with-jira/releases/tag/v1.0.0

