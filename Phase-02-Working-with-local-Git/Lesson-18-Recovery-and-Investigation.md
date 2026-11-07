# Lesson 18: Recovery and Investigation with Git Reflog

## Learning objectives
- Understand what Git reflog records.
- Investigate previous HEAD positions.
- Find commits that disappeared from normal branch history.
- Recover access to previous commits.

## Core idea

`git reflog` records changes in the positions of Git references, especially HEAD.

It helps investigate previous states of a repository and locate commits that are no longer visible in normal Git history.

## Important commands

### 1. View reflog

```bash
git reflog
```

### 2. View a shorter reflog

```bash
git reflog --oneline
```

### 3. Inspect a commit

```bash
git show <commit-id>
```

### 4. Create a recovery branch

```bash
git branch recovery-branch <commit-id>
```

This creates a branch pointing to the selected commit without moving the current branch.

### 5. Switch to the recovery branch

```bash
git switch recovery-branch
```

## Git log vs Git reflog

| Git log | Git reflog |
|---|---|
| Shows commit history reachable from the selected reference | Records previous movements of references |
| Helps inspect project history | Helps investigate previous repository states |
| Does not normally show commits abandoned by branch movement | Can help locate those commits |

## Safety notes
- Reflog is local, not a remote backup.
- Reflog entries can expire.
- Avoid experimenting with destructive reset commands in important repositories.
- Create a recovery branch when you need to preserve access to a previous commit.

## What I learned

Git reflog helps investigate previous HEAD positions and recover access to commits that are no longer visible in normal branch history.