# Lesson 29: Remote Names and URLs

## Learning Objectives
- Understand Git remotes.
- Understand remote names and URLs.
- Learn how to inspect remote connections.
- Learn how to add, update, and remove remote references.

## Core Idea
A Git remote is a reference to another repository hosted somewhere outside your local computer.

A remote has a name and a URL.

The most common remote name is `origin`.

## Why It Matters
Remote configuration allows Git to know where to retrieve changes from and where to send local commits.

## Important Git Commands

### 1. List Remote Names

```bash
git remote
```

Displays the configured remote names.

### 2. View Remote URLs

```bash
git remote -v
```

Displays remote names and their fetch and push URLs.

### 3. Add a Remote

```bash
git remote add origin https://github.com/user/project.git
```

Adds a remote reference named `origin`.

### 4. View Detailed Remote Information

```bash
git remote show origin
```

Displays detailed information about a remote.

### 5. Change a Remote URL

```bash
git remote set-url origin NEW_URL
```

Updates the URL associated with a remote name.

### 6. Remove a Remote

```bash
git remote remove origin
```

Removes the remote reference from local Git configuration without deleting the remote repository.

## Understanding Fetch and Push

- **Fetch URL:** Used to retrieve information from a remote.
- **Push URL:** Used to send commits to a remote.

These URLs are commonly identical.

## How Cloning Uses Remotes

When you clone a repository, Git normally creates a remote named `origin` pointing to the repository you cloned.

## Practical Demonstration

Inspect your learning repository:

```powershell
git remote
git remote -v
git remote show origin
```

Record the remote name, URL, and fetch/push configuration.

## Common Mistakes and Safety Notes
- `origin` is a conventional name, not a special Git command.
- Do not confuse a remote name with its URL.
- Removing a remote does not delete the GitHub repository.
- Check the URL before pushing commits.

## Practice Task
1. Inspect configured remote names.
2. Display remote URLs.
3. Inspect detailed remote information.
4. Identify the fetch and push URLs.
5. Do not modify your remote configuration during this exercise.

## Knowledge Check
1. What is `origin`?
2. Which command displays remote names and URLs?
3. What does `git remote set-url` do?
4. Does removing a remote delete the GitHub repository?

## What I Learned
Git remotes allow local repositories to connect to remote repositories. Remote names such as `origin` provide convenient references to repository URLs.