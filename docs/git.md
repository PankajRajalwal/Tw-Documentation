# Git and GitHub

This page follows the class handout **Version Control Tools: Git and GitHub** by Prof. Neeta Nain, MNIT Jaipur, 12 October 2026.

## 1. Introduction to Version Control

Version control is a system that records changes made to files over time. It helps developers track history, compare versions, restore previous versions, and collaborate.

## 2. Git and GitHub

- **Git:** A distributed version control system.
- **GitHub:** An online hosting and collaboration platform for Git repositories.

## 3. Installing Git on macOS

Install Git using Homebrew:

```bash
brew install git
```

Verify installation:

```bash
git --version
```

## 4. Git Configuration

Set username and email:

```bash
git config --global user.name "PankajRajalwal"
git config --global user.email "YOUR_COLLEGE_EMAIL"
git config --global --list
```

## 5. Creating a Repository

```bash
mkdir my-project
cd my-project
git init
```

## 6. Basic Git Workflow

Git has three main areas:

1. Working Directory
2. Staging Area
3. Repository

Commands:

```bash
git status
git add filename
git add .
git commit -m "Add project files"
```

## 7. Checking History and Differences

```bash
git log
git log --oneline
git diff
git diff --staged
git diff HEAD
git ls-files

## 8. Using .gitignore

The `.gitignore` file tells Git which files and folders should not be tracked.

Example:

```gitignore
.DS_Store
*.log
build/