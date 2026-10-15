# Git Commands Reference

## 1. Setup & Config

### Check Git Version
- **Command:** `git --version`
- **What it does:** Displays the installed Git version.
- **Example:** `git --version`

### Configure Git Username
- **Command:** `git config --global user.name`
- **What it does:** Sets the name recorded as the author of your commits.
- **Example:** `git config --global user.name "Devesh Arya"`

### Configure Git Email
- **Command:** `git config --global user.email`
- **What it does:** Sets the email address recorded in your commits.
- **Example:** `git config --global user.email "your-email@example.com"`

### View Git Configuration
- **Command:** `git config --list`
- **What it does:** Displays Git configuration settings.
- **Example:** `git config --list`



## 2. Basic Workflow

### Create a Directory
- **Command:** `mkdir`
- **What it does:** Creates a new directory.
- **Example:** `mkdir devops-git-practice`

### Change Directory
- **Command:** `cd`
- **What it does:** Changes the current working directory.
- **Example:** `cd devops-git-practice`

### Initialize a Repository
- **Command:** `git init`
- **What it does:** Initializes a Git repository in the current directory.
- **Example:** `git init`

### Create a File
- **Command:** `touch`
- **What it does:** Creates an empty file.
- **Example:** `touch git-commands.md`

## 3. Viewing Changes

### Check Repository Status
- **Command:** `git status`
- **What it does:** Shows the current branch and file tracking status.
- **Example:** `git status`

### Display Current Directory
- **Command:** `pwd`
- **What it does:** Displays the current directory path.
- **Example:** `pwd`

### List All Files
- **Command:** `ls -la`
- **What it does:** Lists files, including hidden files and directories.
- **Example:** `ls -la`

### Explore Git Metadata
- **Command:** `ls -la .git`
- **What it does:** Lists the contents of Git's internal metadata directory.
- **Example:** `ls -la .git`

### Inspect HEAD
- **Command:** `cat .git/HEAD`
- **What it does:** Displays the reference to the current branch or commit.
- **Example:** `cat .git/HEAD`

### Display Current Branch
- **Command:** `git branch --show-current`
- **What it does:** Displays the current branch name.
- **Example:** `git branch --show-current`

### Display Repository Root
- **Command:** `git rev-parse --show-toplevel`
- **What it does:** Displays the root directory of the current repository.
- **Example:** `git rev-parse --show-toplevel`

---

## Summary
These commands cover Git installation, configuration, repository initialization, file creation, and repository inspection.


## 4. Staging and Inspecting Changes

### Stage a File
- **Command:** `git add`
- **What it does:** Adds file changes to the staging area.
- **Example:** `git add git-commands.md`

### View Unstaged Changes
- **Command:** `git diff`
- **What it does:** Shows changes in tracked files that are not staged.
- **Example:** `git diff`

### View Staged Changes
- **Command:** `git diff --cached`
- **What it does:** Shows changes staged for the next commit.
- **Example:** `git diff --cached`

## 5. Commits and History

### Create a Commit
- **Command:** `git commit -m`
- **What it does:** Saves staged changes as a new commit.
- **Example:** `git commit -m "Update Git reference"`

### View Commit History
- **Command:** `git log`
- **What it does:** Displays detailed commit history.
- **Example:** `git log`

### View Compact History
- **Command:** `git log --oneline`
- **What it does:** Displays each commit on a single line.
- **Example:** `git log --oneline`

### Inspect the Latest Commit
- **Command:** `git show`
- **What it does:** Displays details and changes from a commit.
- **Example:** `git show HEAD`

## 6. Branches and Repository Information

### List Local Branches
- **Command:** `git branch`
- **What it does:** Lists local branches.
- **Example:** `git branch`

### Create a Branch
- **Command:** `git branch <branch-name>`
- **What it does:** Creates a new branch without switching to it.
- **Example:** `git branch feature/docs`

### Show Repository Root
- **Command:** `git rev-parse --show-toplevel`
- **What it does:** Displays the root path of the current repository.
- **Example:** `git rev-parse --show-toplevel`

### View Remote Repositories
- **Command:** `git remote -v`
- **What it does:** Lists configured remote repositories and their URLs.
- **Example:** `git remote -v`
