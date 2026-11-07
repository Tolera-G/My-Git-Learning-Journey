# Lesson 15: Undoing Safely

## Learning objectives
- Understand how to unstage changes.
- Understand how to discard unstaged modifications.
- Recognize the difference between safe and destructive undo operations.

## Core idea

Git provides different commands for undoing changes depending on where those changes exist.

## Important commands

### 1. Unstage changes

```bash
git restore --staged filename
```

Removes changes from the staging area while keeping the modifications in the working directory.

### 2. Discard unstaged changes

```bash
git restore filename
```

Restores the working-directory file to its staged version. Any unstaged modifications are discarded.

### 3. Check repository status

```bash
git status
```

Shows which changes are staged, unstaged, or untracked.

## Key difference

| Command | Result |
|---|---|
| `git restore --staged file` | Unstages changes |
| `git restore file` | Discards unstaged changes |
| `git status` | Checks repository state |

## Safety notes
- Always inspect `git status` before undoing changes.
- Use `git diff` to inspect unstaged changes.
- Use `git diff --staged` to inspect staged changes.
- Be careful with `git restore` because it can permanently discard modifications.

## What I learned

Undoing changes in Git requires understanding where those changes are stored. Unstaging preserves work, while restoring a file can discard unstaged modifications.