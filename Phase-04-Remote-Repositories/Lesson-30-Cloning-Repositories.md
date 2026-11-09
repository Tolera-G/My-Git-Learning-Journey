# Lesson 30: Cloning Repositories

## Learning objectives
- Understand what repository cloning means.
- Use `git clone` to copy a remote repository.
- Understand the difference between cloning and downloading a ZIP file.
- Verify a cloned repository.

## Core idea
Cloning creates a local copy of an existing remote Git repository on your computer.

## Why it matters
Cloning allows developers to work with existing projects, contribute to other repositories, and collaborate with team members.

## How it works
When Git clones a repository, it normally downloads:
- Project files and folders.
- Commit history.
- Branch information.
- Remote configuration, including the default remote named `origin`.

## Practical demonstration

```powershell
git clone https://github.com/OWNER/REPOSITORY.git
cd REPOSITORY
git status
git log --oneline -5
git remote -v
```

## Common mistakes and safety notes
- Do not clone into an existing non-empty folder.
- Enter the cloned directory before running Git commands.
- Cloning does not automatically grant permission to push changes.
- Downloading a ZIP file does not provide Git history or remote configuration.

## Practice task
1. Clone a GitHub practice repository.
2. Enter its local folder.
3. Inspect its status and commit history.
4. Verify its remote URL using `git remote -v`.

## Knowledge check
1. What is the difference between `git init` and `git clone`?
2. Why does Git normally create a remote named `origin`?
3. What does cloning provide that downloading a ZIP file does not?

## What I learned
Cloning allows me to create a local Git copy of an existing remote repository while keeping its history and remote connection.
