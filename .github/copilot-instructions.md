# GitHub Organization Repository (.github)

The arisecloudsolutions/.github repository is a GitHub organization-level special repository used to store organization-wide configuration files, templates, and documentation that apply across all repositories in the organization.

Always reference these instructions first and fallback to search or bash commands only when you encounter unexpected information that does not match the info here.

## Working Effectively

### Repository Structure and Purpose
This is a special GitHub organization repository with the following structure:
- `README.md` - Organization profile displayed on the organization's GitHub page
- `.github/` - Directory containing organization-wide GitHub configuration
  - `ISSUE_TEMPLATE/` - Issue templates applied to all organization repositories
  - `workflows/` - Workflow templates available to all organization repositories
- `profile/` - Organization profile assets and documentation
- Additional organization-wide configuration files

### Basic Operations
- Clone repository: `git clone https://github.com/arisecloudsolutions/.github.git`
- All file operations work instantly (< 5ms execution time)
- All git operations work instantly (< 10ms execution time)
- No build process required - this repository contains only configuration files and documentation

### Required Tools and Dependencies
- Git (pre-installed and configured)
- Standard text editors and file manipulation tools
- Node.js, npm, yarn, and Python 3.12.3 are available but typically not needed
- No additional dependencies required for basic operations

### Validation and Testing
- File operations: Create, edit, delete markdown and YAML files work correctly
- Git operations: add, commit, reset, status all function properly
- Directory operations: Create and manage standard organization repository directories
- README.md editing: Safe to edit organization profile content

### Common Tasks and Commands
- Edit organization profile: Modify `README.md` in repository root
- Add issue templates: Create files in `.github/ISSUE_TEMPLATE/`
- Add workflow templates: Create files in `.github/workflows/`
- Test changes: `git status && git diff` to review modifications
- Validate markdown: Use standard text editors (no specific linting tools available)

## Validation Requirements

### Before Making Changes
- Always run `git status` to check repository state
- Verify you're on the correct branch: `git branch -a`
- Review current content: `cat README.md` or relevant files

### After Making Changes
- Always validate file syntax by viewing created/edited files
- Run `git status` to confirm expected changes
- Use `git diff` to review specific modifications
- Test file operations work correctly with sample content

### Repository-Specific Validation
- Organization README changes: Verify HTML entities are properly escaped (e.g., `&amp;` for `&`)
- Issue templates: Ensure YAML front matter is properly formatted
- Workflow templates: Validate YAML syntax for GitHub Actions
- Profile assets: Confirm files are in appropriate formats and sizes

## Critical Guidelines

### File Management
- NEVER delete existing files without explicit requirement
- Always backup critical files before major changes: `cp README.md README.md.backup`
- Use proper file extensions: `.md` for Markdown, `.yml` for YAML
- Follow GitHub naming conventions for template files

### Git Workflow
- Commit changes atomically with descriptive messages
- Always review changes with `git diff` before committing
- Use `git add -A` to stage all changes or `git add <specific-file>`
- Repository operations are instant - no timeout concerns needed

### Organization Repository Best Practices
- Keep README.md concise and professional for organization profile
- Use consistent formatting and style across all templates
- Test template functionality in test repositories when possible
- Document any organization-specific conventions or requirements

## Timing Expectations
- File operations: Instant (< 5ms)
- Git operations: Instant (< 10ms)
- No build or compilation steps required
- NEVER CANCEL: Not applicable - all operations complete instantly

## Error Prevention
- Always verify markdown syntax before committing
- Check YAML file formatting for issue and workflow templates
- Confirm file permissions allow read/write operations
- Validate directory structure matches GitHub organization conventions
- Test that templates render correctly in GitHub interface when possible

## Directory Reference
```
/home/runner/work/.github/.github/
├── .git/                    # Git repository data
├── .github/                 # Organization-wide GitHub configuration
│   ├── ISSUE_TEMPLATE/      # Issue templates for all org repos
│   └── workflows/           # Workflow templates for all org repos
├── profile/                 # Organization profile assets
└── README.md               # Organization profile (displayed on GitHub)
```

## Quick Command Reference
- Repository status: `git status`
- View changes: `git diff`
- List files: `ls -la`
- Edit README: Use any text editor on `README.md`
- Create template: Create file in appropriate `.github/` subdirectory
- Validate content: `cat <filename>` to review file contents
- Timing test: `time <command>` (all operations complete in milliseconds)