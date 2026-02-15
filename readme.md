# Git Tutorial

A hands-on tutorial repository for learning Git version control fundamentals, created as part of the freeCodeCamp curriculum.

## Overview

This repository serves as a practical learning environment for understanding Git concepts including:

- Repository initialization
- Staging and committing changes
- Branch management
- Remote repository operations
- Collaboration workflows

## Prerequisites

Before starting this tutorial, ensure you have:

- Git installed on your system ([Download Git](https://git-scm.com/downloads))
- A GitHub account ([Sign up](https://github.com/signup))
- Basic terminal/command line knowledge

## Getting Started

### Clone the Repository

```bash
git clone git@github.com:AungMyoKyaw/fcc-git-tutorial.git
cd fcc-git-tutorial
```

### Basic Git Commands

| Command | Description |
|---------|-------------|
| `git init` | Initialize a new Git repository |
| `git status` | Show working tree status |
| `git add <file>` | Stage file(s) for commit |
| `git commit -m "message"` | Commit staged changes |
| `git push` | Push commits to remote |
| `git pull` | Fetch and merge remote changes |
| `git branch <name>` | Create a new branch |
| `git checkout <branch>` | Switch to a branch |
| `git merge <branch>` | Merge branch into current |

## Project Structure

```
fcc-git-tutorial/
├── readme.md       # Project documentation
└── .gitignore      # Git ignore patterns
```

## Common Git Workflows

### Feature Branch Workflow

```bash
# Create and switch to a new feature branch
git checkout -b feature/my-new-feature

# Make changes and stage them
git add .

# Commit with a descriptive message
git commit -m "feat: add new feature"

# Push to remote
git push -u origin feature/my-new-feature
```

### Syncing with Remote

```bash
# Fetch latest changes without merging
git fetch origin

# Pull and merge latest changes from main branch
git pull origin master

# Rebase your branch on top of latest master
git rebase origin/master
```

## Best Practices

- **Commit often**: Small, focused commits are easier to review and revert
- **Write clear messages**: Use conventional commit format (feat, fix, docs, style, refactor, test, chore)
- **Pull before push**: Always sync with remote before pushing
- **Use branches**: Keep master/main stable, develop features in branches
- **Review changes**: Use `git diff` before committing to review your changes

## Troubleshooting

### Undo last commit (keep changes)

```bash
git reset --soft HEAD~1
```

### Discard all local changes

```bash
git checkout -- .
```

### Fix commit message (before push)

```bash
git commit --amend -m "New commit message"
```

### Resolve merge conflicts

```bash
# After resolving conflicts in your editor
git add .
git commit -m "resolve merge conflicts"
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'feat: add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Resources

- [freeCodeCamp](https://www.freecodecamp.org/)
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com/)
- [Pro Git Book](https://git-scm.com/book/en/v2)

## License

This project is open source and available under the [MIT License](LICENSE).

## Author

**Aung Myo Kyaw**

- GitHub: [@AungMyoKyaw](https://github.com/AungMyoKyaw)
