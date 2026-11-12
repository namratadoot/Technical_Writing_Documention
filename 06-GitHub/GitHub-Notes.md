
# GitHub – Notes

## 1. Introduction

GitHub is a platform for hosting Git repositories and collaborating with developers.

It allows developers to:
- Store projects online.
- Share code.
- Review changes.
- Collaborate using branches and pull requests.

## 2. Git vs GitHub

| Git | GitHub |
|---|---|
| Version control system | Hosting and collaboration platform |
| Works locally | Hosts repositories online |
| Tracks project changes | Supports sharing and collaboration |

## 3. Connecting a Local Repository to GitHub

A remote connects a local Git repository to a repository hosted on another system.

```bash
git remote add origin REPOSITORY_URL
```

- `git remote add`: Adds a remote connection.
- `origin`: Conventional remote name.
- `REPOSITORY_URL`: URL of the hosted repository.

Check configured remotes:

```bash
git remote -v
```

## 4. Cloning a Repository

Cloning creates a local copy of a remote repository, including its Git history.

```bash
git clone REPOSITORY_URL
```

Cloning downloads repository files and history and configures the original repository as a remote named `origin`.

## 5. Pushing Changes to GitHub

```bash
git branch -M main
git push -u origin main
```

- `git branch -M main`: Renames the current branch to main.
- `git push`: Sends local commits to a remote.
- `-u`: Sets the upstream tracking relationship.

A configured remote and required authentication are needed.

## 6. Fetching and Pulling Changes

Fetch:

```bash
git fetch origin
```

Downloads remote updates without integrating them into the current branch.

Pull:

```bash
git pull
git pull origin main
```

Fetches and integrates remote changes into the current branch.

## 7. Pull Request Workflow

A pull request is used to review changes before integrating them.

Steps:
1. Create a feature branch.
2. Modify and test the code.
3. Stage and commit changes.
4. Push the feature branch to GitHub.
5. Open a pull request.
6. Review the changes.
7. Merge the approved changes.

## 8. Updating the Local Main Branch

After a pull request is merged:

```bash
git switch main
git pull origin main
```

This switches to the main branch and obtains the merged changes.

## 9. Complete GitHub Workflow

```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin REPOSITORY_URL
git push -u origin main
```

This publishes local commits to the configured GitHub repository.

## 10. Complete Developer Workflow

Create or clone repository → Create branch → Modify and test → Stage and commit → Push branch → Open pull request → Review → Merge.
