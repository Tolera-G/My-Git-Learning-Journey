# Lesson 32: Fetching Changes from a Remote Repository

## Learning objectives
- Understand what fetching means.
- Download remote updates using `git fetch`.
- Understand remote-tracking branches.
- Distinguish fetching from pulling.

## Core idea
Fetching downloads updates and new commit information from a remote repository without automatically integrating them into the current local branch.

## Why it matters
Fetching helps developers check remote changes before deciding whether and how to integrate them into their local work.

## How it works
When you fetch from `origin`, Git updates remote-tracking references such as `origin/main`.

Your local branch, such as `main`, and your working files are not automatically updated.

## Practical demonstration

```powershell
git fetch origin
git status -sb
git log --oneline main -5
git log --oneline origin/main -5
git diff main origin/main
```

To see commits available remotely but not locally:

```powershell
git log --oneline main..origin/main
```

## Common mistakes and safety notes
- Fetching does not automatically merge remote changes.
- `main` is a local branch; `origin/main` is a remote-tracking branch.
- Fetching does not automatically change working files.
- Inspect remote changes before integrating them.

## Practice task
1. Make a small README change directly on GitHub.
2. Run `git fetch origin` locally.
3. Inspect the local and remote-tracking branches.
4. Identify any commits that are available remotely but not locally.

## Knowledge check
1. What does `git fetch` do?
2. Does fetching automatically change working files?
3. What is the difference between `main` and `origin/main`?
4. Why might a developer fetch before pulling?

## What I learned
`git fetch` allows me to retrieve remote updates and inspect them before integrating them into my local branch.
