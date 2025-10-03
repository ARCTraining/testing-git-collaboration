# Git Commands Quick Reference

This guide provides quick reference for the most common Git commands you'll use in this workshop.

## 📥 Getting Started

### Clone a Repository
```bash
git clone <repository-url>
```
Downloads a copy of the repository to your local machine.

### Check Repository Status
```bash
git status
```
Shows which files have been modified, staged, or are untracked.

## 🌿 Working with Branches

### List Branches
```bash
git branch              # List local branches
git branch -a           # List all branches (local and remote)
```

### Create a New Branch
```bash
git branch <branch-name>           # Create branch
git checkout <branch-name>         # Switch to branch
# OR do both at once:
git checkout -b <branch-name>      # Create and switch
```

### Switch Branches
```bash
git checkout <branch-name>
```

### Delete a Branch
```bash
git branch -d <branch-name>        # Delete local branch (safe)
git branch -D <branch-name>        # Force delete local branch
```

## 💾 Making Changes

### Stage Files
```bash
git add <file>                     # Stage a specific file
git add .                          # Stage all changes
git add *.md                       # Stage all markdown files
```

### Commit Changes
```bash
git commit -m "Your commit message"
```

### View Changes
```bash
git diff                           # Show unstaged changes
git diff --staged                  # Show staged changes
git diff <branch-name>             # Compare with another branch
```

## ☁️ Working with Remote Repositories

### View Remotes
```bash
git remote -v                      # List remote repositories
```

### Add a Remote
```bash
git remote add <name> <url>        # Add a new remote
```

### Fetch and Pull
```bash
git fetch origin                   # Download changes without merging
git pull origin <branch-name>      # Fetch and merge changes
```

### Push Changes
```bash
git push origin <branch-name>      # Push branch to remote
git push -u origin <branch-name>   # Push and set upstream
```

## 📜 Viewing History

### View Commit History
```bash
git log                            # Full log
git log --oneline                  # Compact log
git log --graph                    # Visual graph
git log -n 5                       # Last 5 commits
```

### View a Specific Commit
```bash
git show <commit-hash>
```

## 🔄 Synchronizing

### Update Your Fork
```bash
# Add upstream remote (only once)
git remote add upstream <original-repo-url>

# Fetch and merge updates
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```

## ⚠️ Undoing Changes

### Discard Changes in Working Directory
```bash
git checkout -- <file>             # Discard changes to a file
git checkout -- .                  # Discard all changes
```

### Unstage Files
```bash
git reset HEAD <file>              # Unstage a specific file
git reset HEAD                     # Unstage all files
```

### Amend Last Commit
```bash
git commit --amend -m "New message"  # Change last commit message
```

## 🆘 Getting Help

### Command Help
```bash
git help                           # General help
git help <command>                 # Help for specific command
git <command> --help               # Alternative help format
```

## 💡 Tips and Best Practices

### Commit Messages
- Use present tense: "Add feature" not "Added feature"
- Be specific and concise
- Start with a verb: Add, Update, Fix, Remove

### Branch Names
- Use lowercase and hyphens
- Be descriptive: `add-my-profile`, `fix-readme-typo`
- Avoid spaces and special characters

### Workflow
1. Always `git pull` before starting new work
2. Create a new branch for each feature/fix
3. Commit often with meaningful messages
4. Push regularly to backup your work
5. Keep commits focused and atomic

## 🔗 Additional Resources

- [Official Git Documentation](https://git-scm.com/doc)
- [GitHub Git Cheat Sheet](https://training.github.com/downloads/github-git-cheat-sheet/)
- [Interactive Git Tutorial](https://learngitbranching.js.org/)
- [Visualizing Git Concepts](https://git-school.github.io/visualizing-git/)

---

Keep this reference handy as you work through the workshop!
