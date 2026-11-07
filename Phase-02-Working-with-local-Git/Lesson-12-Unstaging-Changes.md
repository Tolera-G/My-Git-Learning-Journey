# Lesson 12: Unstaging Changes with git restore --staged

## 1. Learning Objectives
- Understand how to unstage changes.
- Use `git restore --staged`.
- Distinguish unstaging from deleting or discarding changes.

## 2. What Is Unstaging?
Unstaging means removing changes from the staging area without deleting the changes from your files.

The changes return to the working directory as unstaged modifications.

## 3. The git restore --staged Command

To unstage a specific file:

```bash
git restore --staged index.html
```

This removes the file's staged changes from the next commit's preparation list.

## 4. Checking the Result

Run:

```bash
git status
```

Before unstaging, the file appears under:

`Changes to be committed`

After unstaging, it appears under:

`Changes not staged for commit`

## 5. Important Difference

- `git restore --staged file`: Unstages changes.
- `git restore file`: Discards unstaged modifications.
- `git rm file`: Removes a tracked file and stages its deletion.

Be careful: `git restore file` can permanently discard uncommitted changes.

## 6. What You Learned
- Staged changes can be removed from the staging area.
- `git restore --staged` preserves file modifications.
- `git status` verifies whether changes are staged or unstaged.