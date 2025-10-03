# Git & GitHub Collaboration Workshop

Welcome to the Git & GitHub Collaboration Workshop! This repository is designed to help you learn and practice collaborative Git workflows using GitHub.

## 🎯 Learning Objectives

By the end of this workshop, you will be able to:
- Fork a repository and clone it to your local machine
- Create branches and make changes
- Commit your work with meaningful messages
- Push changes to your fork
- Create and manage pull requests
- Review and merge contributions from others
- Resolve basic merge conflicts

## 📋 Prerequisites

Before starting this workshop, you should have:
- A GitHub account ([Sign up here](https://github.com/join))
- Git installed on your computer ([Installation guide](https://git-scm.com/downloads))
- A text editor (VS Code, Sublime Text, Atom, or any editor you prefer)
- Basic familiarity with command line/terminal

## 🚀 Workshop Structure

This workshop will guide you through a typical collaborative workflow:

1. **Fork & Clone**: Get your own copy of the repository
2. **Branch**: Create a feature branch for your work
3. **Edit**: Make changes to markdown files
4. **Commit**: Save your changes with descriptive messages
5. **Push**: Upload your changes to GitHub
6. **Pull Request**: Propose your changes to the main repository
7. **Review**: Learn to review and provide feedback
8. **Merge**: Integrate approved changes

## 📝 Workshop Instructions

### Step 1: Fork the Repository

1. Click the "Fork" button at the top right of this repository
2. This creates your own copy of the repository under your GitHub account

### Step 2: Clone Your Fork

```bash
# Replace YOUR-USERNAME with your GitHub username
git clone https://github.com/YOUR-USERNAME/testing-git-collaboration.git
cd testing-git-collaboration
```

### Step 3: Create a Branch

Always create a new branch for your changes:

```bash
# Create and switch to a new branch
git checkout -b add-my-introduction
```

Branch naming tips:
- Use descriptive names (e.g., `add-profile`, `fix-typo`)
- Use lowercase and hyphens
- Be concise but clear

### Step 4: Make Your Changes

Add your introduction to the repository:

1. Navigate to the `participants/` directory
2. Copy the `template.md` file and rename it to `your-name.md`
3. Edit the file with your information
4. Save your changes

### Step 5: Commit Your Changes

```bash
# Check what files have changed
git status

# Stage your new file
git add participants/your-name.md

# Commit with a meaningful message
git commit -m "Add introduction for [Your Name]"
```

Good commit message practices:
- Start with a verb (Add, Update, Fix, Remove)
- Be specific about what changed
- Keep it under 50 characters for the first line

### Step 6: Push to Your Fork

```bash
# Push your branch to your fork
git push origin add-my-introduction
```

### Step 7: Create a Pull Request

1. Go to your fork on GitHub
2. Click "Compare & pull request" button
3. Fill in the PR template with:
   - A clear title
   - Description of your changes
   - Any relevant context
4. Click "Create pull request"

### Step 8: Collaborate and Iterate

- Respond to review comments
- Make additional commits if needed
- Keep communication friendly and professional

## 🤝 Collaboration Guidelines

- **Be respectful**: Everyone is learning
- **Be constructive**: Provide helpful feedback
- **Be patient**: Reviews take time
- **Ask questions**: No question is too small
- **Have fun**: Learning should be enjoyable!

## 📚 Additional Resources

- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)
- [Git Handbook](https://guides.github.com/introduction/git-handbook/)
- [Markdown Syntax](https://guides.github.com/features/mastering-markdown/)
- [How to Write Good Commit Messages](https://chris.beams.io/posts/git-commit/)

## 🆘 Getting Help

If you encounter issues:
1. Check the workshop materials
2. Ask your instructor or teaching assistant
3. Search GitHub issues in this repository
4. Create a new issue with the `question` label

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Happy collaborating! 🎉
