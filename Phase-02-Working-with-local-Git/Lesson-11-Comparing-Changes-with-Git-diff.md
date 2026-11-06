# Lesson 11: Comparing Changes with git diff

## 1. Learning Objectives
- Understand the purpose of `git diff`.
- Identify added and removed lines.
- Compare unstaged and staged changes.
- Compare two commits.

## 2. What Is git diff?
`git diff` is a Git command used to compare changes between different versions or states of files.

It helps developers understand exactly what has changed.

## 3. Understanding Diff Symbols

```diff
- Old line
+ New line
```

- `+` represents an added line.
- `-` represents a removed line.

## 4. Important git diff Commands

### Compare Unstaged Changes

```bash
git diff
```

Shows changes in the working directory that have not been staged.

### Compare Staged Changes

```bash
git diff --staged
```

Shows changes staged for the next commit compared with the last commit.

### Compare Two Commits

```bash
git diff commit1 commit2
```

Compares the content of two commits.

## 5. What You Learned
- `git diff` helps inspect changes.
- `+` indicates added lines.
- `-` indicates removed lines.
- `git diff` shows unstaged changes.
- `git diff --staged` shows staged changes.