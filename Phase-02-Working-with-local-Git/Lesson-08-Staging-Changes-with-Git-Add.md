# Lesson 08: Staging Changes with git add

## 1. Learning Objectives
- Understand what staging means.
- Learn how to use `git add`.
- Stage individual files and multiple changes.
- Verify staged changes using `git status`.

## 2. What Is Staging?
Staging is the process of selecting changes that will be included in the next commit.

Git uses the staging area as a preparation area between the working directory and the local repository.

## 3. The git add Command

Stage one specific file:

```bash
git add index.html
```

Stage all changes under the current directory:

```bash
git add .
```

## 4. Checking Staged Changes

After staging, run:

```bash
git status
```

Git displays staged changes under:

`Changes to be committed`

## 5. Important Points
- `git add` stages changes.
- Staging does not create a commit.
- You can stage individual files or multiple changes.
- `git status` helps verify what is staged.

## 6. What You Learned
Staging allows you to choose exactly which changes should be included in your next commit.