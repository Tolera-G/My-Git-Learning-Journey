# Lesson 33: Pulling Changes from a Remote Repository

## Learning objectives
- Understand what pulling means.
- Retrieve and integrate remote changes.
- Understand the difference between fetching and pulling.
- Recognize why merge conflicts can occur.

## Core idea
Pulling downloads changes from a remote repository and integrates them into the current local branch.

## Why it matters
When working with other developers, their changes may be pushed to GitHub while you are working locally. Pulling helps you receive and integrate those changes.

## How it works
A normal `git pull` performs two main operations:

1. Fetches updates from the remote repository.
2. Integrates those updates into the current branch, usually by merging.

## Practical demonstration

```powershell
git status
git pull origin main
git log --oneline -5
```

## Fetch vs Pull

- `git fetch` downloads remote updates without automatically integrating them into the current branch.
- `git pull` downloads remote updates and integrates them into the current branch.

## Common mistakes and safety notes
- Check your working tree before pulling.
- Commit or safely set aside unfinished changes.
- Verify the remote and branch names.
- A merge conflict can happen when changes overlap.
- Avoid destructive commands when troubleshooting pull errors.

## Practice task
1. Make a README change directly on GitHub.
2. Commit the change on GitHub.
3. Pull the changes into your local repository.
4. Verify that the README contains the new content.

## Knowledge check
1. What does `git pull` do?
2. What are its two main operations?
3. What is the difference between fetch and pull?
4. Why check `git status` before pulling?
5. What is a merge conflict?

## What I learned
`git pull` allows me to retrieve and integrate changes from a remote repository into my local branch.
