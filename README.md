# GitHub Achievement Automation 🦈🧠

This repository is set up to automatically generate achievements for both **Pull Shark** and **Galaxy Brain** through automated workflows and discussions.

## 🦈 Pull Shark Automation

### How It Works
- **Auto PR Generator**: Creates dummy PRs twice daily (every 12 hours)
- **CI Workflow**: Runs basic tests that always pass
- **Auto Merge**: Automatically merges PRs once CI passes
- **Dependabot**: Generates additional PRs for dependency updates

### Pull Shark Levels
- 🦈 **Level 1**: 2 merged PRs
- 🦈 **Level 2**: 16 merged PRs  
- 🦈 **Level 3**: 128 merged PRs
- 🦈 **Level 4**: 1024 merged PRs

## 🧠 Galaxy Brain Automation

### How It Works
- **Auto Discussion Creator**: Posts questions every 6 hours using helper account
- **Auto Answer Bot**: Responds with helpful answers using your main account
- **Auto Acceptance**: Helper account marks answers as accepted
- **Content Variety**: 8 different Q&A pairs for natural variety

### Galaxy Brain Levels
- 🧠 **Level 1**: 1 accepted answer
- 🧠 **Level 2**: 2 accepted answers
- 🧠 **Level 3**: 3 accepted answers
- 🧠 **Level 4**: 4 accepted answers

## 🚀 Setup

### Prerequisites
1. Push this repository to GitHub
2. Enable Actions in repository settings
3. Enable Discussions in repository settings
4. Create at least one discussion category

### Required Secrets
- `HELPER_TOKEN`: GitHub token from helper account (creates discussions, accepts answers)
- `ACTIONS_BOT_TOKEN`: GitHub token from your main account (posts answers)

### Token Permissions
Both tokens need:
- `repo` scope (full control of private repositories)
- `write:discussion` scope (create and manage discussions)

## 📋 Workflows

### Pull Shark Workflows
- `.github/workflows/auto-prs.yml` - Generates PRs on schedule
- `.github/workflows/ci.yml` - Basic CI testing
- `.github/workflows/auto-merge.yml` - Auto-merges passing PRs

### Galaxy Brain Workflows
- `.github/workflows/galaxy-brain.yml` - Creates discussions, posts answers, marks as accepted

### Other
- `.github/dependabot.yml` - Dependency update PRs

## ⏰ Schedule

- **Pull Shark**: PRs generated every 12 hours
- **Galaxy Brain**: Discussions created every 6 hours
- **Manual Triggers**: All workflows can be run manually

## 🎯 Achievement Strategy

### Pull Shark
- PRs are generated every 12 hours to avoid GitHub throttling
- All PRs are automatically merged if CI passes
- Mix in real work to maintain natural account activity

### Galaxy Brain
- Questions and answers are varied and helpful
- Automation respects GitHub API rate limits
- Discussions provide genuine value to the community

## 🔒 Safety & Ethics

- **Rate Limiting**: Conservative schedules to maintain good standing with GitHub
- **Content Quality**: Questions and answers are relevant and helpful
- **Educational Purpose**: Designed for learning GitHub automation
- **Community Value**: Discussions contribute positively to the repository

## 📝 Notes

- This is designed for sandbox/testing repositories, not production code
- Both automation systems work independently
- Achievements scale naturally over time
- Monitor GitHub Actions tab for automation status

## 🎉 Success Indicators

### Pull Shark Progress
- Check your GitHub profile for Pull Shark badge
- Monitor PR count in repository
- View merged PRs in Actions tab

### Galaxy Brain Progress
- Check your GitHub profile for Galaxy Brain badge
- View discussions in repository Discussions tab
- Monitor accepted answers count 