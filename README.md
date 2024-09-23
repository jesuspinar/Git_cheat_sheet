# Git Introduction
> A beginner's guide to essential Git commands and configurations.

This guide provides a collection of common Git commands, along with explanations on how to configure and use Git for version control. Whether you're just getting started or need a reference for frequently used commands, this guide is designed to help.

---

## Table of Contents
1. [Global Configuration](#global-configuration)
   - [Set your name](#set-your-name)
   - [Set your email](#set-your-email)
   - [Set default text editor](#set-default-text-editor)
   - [Open Git config settings](#open-git-config-settings)
   - [Set line ending preferences](#set-line-ending-preferences)
2. [Useful Git Commands](#useful-git-commands)
   - [Initialize a Git repository](#initialize-a-git-repository)
   - [Stage changes](#stage-changes)
   - [Make a commit](#make-a-commit)
   - [Remove files](#remove-files)
   - [Rename or move files](#rename-or-move-files)
   - [View status](#view-status)
   - [View differences](#view-differences)
   - [View commit history](#view-commit-history)
   - [Branch management](#branch-management)
   - [Merging changes](#merging-changes)
   - [Working with remotes](#working-with-remotes)

---

## Global Configuration

### Set your name
To configure Git to use your name in commits, run:
```bash
git config --global user.name "Your name"
```

### Set your email
To set the email associated with your Git commits:
```bash
git config --global user.email "name@email.com"
```

### Set default text editor
If you want to set a default text editor, such as VSCode, for commit messages:
```bash
git config --global core.editor "code --wait"
```

### Open Git config settings
To open and edit Git’s global configuration settings:
```bash
git config --global -e
```

### Set line ending preferences
For **Linux/Mac** systems (use Unix-style line endings):
```bash
git config --global core.autocrlf input
```

For **Windows** systems (use Windows-style line endings):
```bash
git config --global core.autocrlf true
```

For other options, you can view the Git configuration help:
```bash
git config -h
```

---

## Useful Git Commands

### Initialize a Git repository
To initialize a new Git repository in the current folder:
```bash
git init
```

### Stage changes
To stage all changes (deleted, modified, and new files):
```bash
git add .
```

### Make a commit
To create a new commit with a message:
```bash
git commit -m "Initial commit"
```

### Remove files
To remove a file from your working tree and stage the removal:
```bash
git rm <file>
```

### Rename or move files
To rename or move a file:
```bash
git mv <old-filename> <new-filename>
```

### View status
To check the status of your working directory:
```bash
git status
```

For a more concise, cleaner output of the status:
```bash
git status -s
```

### View differences
To view the unstaged differences in your working directory:
```bash
git diff
```

To compare the changes already staged for commit:
```bash
git diff --staged
```

### View commit history
To view the commit history:
```bash
git log
```

For a simplified, one-line-per-commit view:
```bash
git log --oneline
```

### Branch management

- To view the current branch:
  ```bash
  git branch
  ```

- To view all local and remote branches:
  ```bash
  git branch -vva
  ```

- To create and switch to a new branch:
  ```bash
  git checkout -b <branch-name>
  ```

- To delete a local branch:
  ```bash
  git branch -d <branch-name>
  ```

- To switch between branches:
  ```bash
  git switch <branch-name>
  ```

### Merging changes
To merge changes from one branch into your current branch:
```bash
git merge <branch-name>
```

### Working with remotes

- To add a remote repository:
  ```bash
  git remote add origin https://github.com/your/repo.git
  ```

- To push changes to a remote branch:
  ```bash
  git push origin <branch-name>
  ```

- If local and remote branch names are different:
  ```bash
  git push origin <local-branch>:<remote-branch>
  ```

- To create and push to a `main` branch:
  ```bash
  git push -u origin main
  ```

- To list, remove, or rename remote repositories:
  ```bash
  git remote -v
  git remote rm <name>
  git remote rename <oldname> <newname>
  ```

- After pulling changes, to view the history of changes:
  ```bash
  git whatchanged
  ```

---

For more details and advanced options, refer to the [Git documentation](https://git-scm.com/doc).
