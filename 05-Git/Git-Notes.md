
# Git – Notes

## 1. Introduction

Git is a version control system that tracks changes in files and projects.

It helps developers:
- Track modifications.
- Maintain commit history.
- Work with branches.
- Manage project versions.

## 2. Creating a Repository

```bash
mkdir my-project
cd my-project
git init
```

- `mkdir`: Creates a directory.
- `cd`: Changes the current directory.
- `git init`: Initializes a Git repository.

## 3. Checking Repository Status

```bash
git status
```

Displays untracked files, modified files, staged changes and working-tree status.

## 4. Tracking and Staging Files

```bash
git add main.py
git add .
```

- `git add`: Stages a file or its changes.
- `git add .`: Stages changes in the current directory.

## 5. Creating Commits

```bash
git commit -m "Add main program"
```

A commit records staged changes in the local repository.

Commit messages should be concise and specific.

Examples:
- Add input validation
- Fix division by zero error
- Update project documentation

## 6. Viewing Commit History

```bash
git log
git log --oneline
```

Displays commit information such as commit hash, author, date and message.

## 7. Comparing Changes

```bash
git diff
git diff --staged
git diff HEAD
```

- `git diff`: Shows unstaged changes.
- `git diff --staged`: Shows staged changes.
- `git diff HEAD`: Shows tracked changes relative to the current commit.

## 8. Branching

A branch is a movable reference to a commit. It allows work to be separated.

```bash
git branch
git branch feature-login
```

- `git branch`: Lists local branches.
- `git branch feature-login`: Creates a new branch.
- The current branch is marked with an asterisk.

## 9. Switching Branches

```bash
git switch feature-login
git switch main
```

Use `git switch` to change the current branch.

Create and switch to a new branch:

```bash
git switch -c feature-login
```

## 10. Merging Branches

Merging integrates changes from one branch into another.

```bash
git switch main
git merge feature-login
```

The target branch is the branch currently checked out.

If Git reports conflicts, resolve them and test the result.
