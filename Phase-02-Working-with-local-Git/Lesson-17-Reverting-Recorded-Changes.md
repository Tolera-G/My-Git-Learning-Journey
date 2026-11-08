# Lesson 17: Reverting Recorded Changes

## Learning objectives
- Understand how `git revert` works.
- Reverse changes introduced by an earlier commit.
- Understand the difference between `git revert` and `git reset`.

## Core idea

`git revert` reverses the changes introduced by a previous commit by creating a new commit.

It does not delete the original commit from history.

## Why it matters

Sometimes a committed change introduces a bug or unwanted result. Reverting allows us to undo that change while preserving the project's commit history.

## Important commands

### 1. View commit history

```bash
git log --oneline
```

### 2. Revert a commit

```bash
git revert <commit-id>
```

### 3. Revert without editing the default message

```bash
git revert --no-edit <commit-id>
```

### 4. Inspect the latest commit

```bash
git show --stat HEAD
```

## Git revert vs Git reset

| Git revert | Git reset |
|---|---|
| Creates a new commit | Moves the current branch pointer |
| Preserves existing history | Can remove commits from current branch history |
| Generally safer for shared history | Requires extra care |

## Safety notes
- Check the commit ID before reverting.
- Inspect the repository status before starting.
- Reverting a commit does not erase that commit from history.
- Reverting older commits can sometimes produce merge conflicts.

## What I learned

Git revert provides a safe way to reverse a recorded change while preserving the original commit and adding a new commit to document the reversal.