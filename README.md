# .github

Shared community health files, issue templates, and GitHub Actions workflows for the **onthisdayph** organization.

Files in this repository are automatically inherited by all repositories in the organization that do not define their own.

## What's Included

### Issue Templates

- **Bug Report** (`ISSUE_TEMPLATE/bug_report.yml`) — Structured form for reporting bugs with steps to reproduce, expected vs. actual behavior, and environment details.
- **Feature Request** (`ISSUE_TEMPLATE/feature_request.yml`) — Structured form for proposing new features with problem statement, proposed solution, and priority.

### Pull Request Template

- **PR Template** (`pull_request_template.md`) — Standardized checklist covering summary, type of change, testing, and review requirements.

### Workflows

- **Release** (`workflows/release.yml`) — Automated release pipeline triggered on pushes to the `production` branch or via manual dispatch. Computes the next semantic version, generates a changelog, creates a release branch (`release/YYYY-MM-DD_vX.Y.Z`), tags the commit, and publishes a GitHub Release.
- **Auto-label Issues** (`workflows/label-issues.yml`) — Automatically applies labels to new issues based on their title prefix (e.g., `[Bug]` or `[Feature]`).

## Usage

These files apply organization-wide by default. To override any file for a specific repository, add the equivalent file to that repository's `.github/` directory.

## Contributing

1. Open an issue using the appropriate template.
2. Submit a pull request following the PR template.
