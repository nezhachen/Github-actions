# Pull Shark Automation 🦈

This repository is set up to automatically generate and merge pull requests to help progress through GitHub's Pull Shark achievement levels.

## How It Works

- **Auto PR Generator**: Creates dummy PRs twice daily (every 12 hours)
- **CI Workflow**: Runs basic tests that always pass
- **Auto Merge**: Automatically merges PRs once CI passes
- **Dependabot**: Generates additional PRs for dependency updates

## Pull Shark Levels

- 🦈 **Level 1**: 2 merged PRs
- 🦈 **Level 2**: 16 merged PRs  
- 🦈 **Level 3**: 128 merged PRs
- 🦈 **Level 4**: 1024 merged PRs

## Setup

1. Push this repository to GitHub
2. Ensure the repository has Actions enabled
3. The workflows will start running automatically

## Workflows

- `.github/workflows/auto-prs.yml` - Generates PRs on schedule
- `.github/workflows/ci.yml` - Basic CI testing
- `.github/workflows/auto-merge.yml` - Auto-merges passing PRs
- `.github/dependabot.yml` - Dependency update PRs

## Notes

- PRs are generated every 12 hours to avoid GitHub throttling
- All PRs are automatically merged if CI passes
- This is designed for sandbox/testing repositories, not production code
- Mix in real work to maintain natural account activity

## Safety

This automation is designed to be sustainable and won't spam GitHub with excessive PRs. The schedule is conservative to maintain good standing with GitHub's systems. 