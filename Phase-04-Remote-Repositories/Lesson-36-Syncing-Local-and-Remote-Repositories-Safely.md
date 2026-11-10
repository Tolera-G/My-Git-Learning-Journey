# Lesson 36: Syncing Local and Remote Repositories Safely

## Learning objectives
- Understand repository synchronization.
- Use fetch, pull, and push together.
- Interpret ahead and behind information.
- Synchronize repositories safely.

## Core idea
Synchronization keeps local and remote repositories up to date by exchanging and integrating commits.

## Why it matters
When multiple developers work on the same project, their local and remote repositories can contain different commits. Synchronization helps keep their work connected.

## How it works

| Command | Purpose |
|---|---|
| `git fetch` | Downloads remote updates without automatically integrating them. |
| `git pull` | Downloads and integrates remote updates. |
| `git push` | Sends local commits to the remote repository. |

## Practical demonstration

```powershell
git status
git branch --show-current
git fetch origin
git status -sb
git pull
git add README.md
git commit -m "Add synchronization notes"
git push
git status
```

## Understanding ahead and behind

- `ahead 1`: One local commit is missing remotely.
- `behind 2`: Two remote commits are missing locally.
- `ahead 1, behind 2`: Both local and remote branches contain commits missing from the other.

## Common mistakes and safety notes
- Always inspect repository status before synchronization.
- Check your current branch.
- Commit or safely stash unfinished changes before integrating remote updates.
- Inspect remote changes when necessary.
- Resolve conflicts carefully.
- Avoid force pushing because it can overwrite remote history.

## Practice task
1. Make a change directly on GitHub.
2. Fetch remote updates locally.
3. Inspect the branch status.
4. Pull the remote changes.
5. Make a local change and commit it.
6. Push the local commit.
7. Verify the final repository status.

## Knowledge check
1. What is repository synchronization?
2. What is the difference between fetch, pull, and push?
3. What does `ahead 1, behind 2` mean?
4. Why might Git reject a push?
5. Why is force pushing dangerous?

## What I learned
Safe synchronization involves checking repository status, retrieving remote updates, integrating changes carefully, and pushing local commits without overwriting other contributors' work.
