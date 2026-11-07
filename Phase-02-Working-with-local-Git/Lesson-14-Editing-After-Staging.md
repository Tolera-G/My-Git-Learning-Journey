# Lesson 14: Editing After Staging

## 1. Learning Objectives
- Understand what happens when a file is edited after staging.
- Identify staged and unstaged changes in the same file.
- Use `git diff` and `git diff --staged` to inspect changes.
- Stage the latest version of a file.

## 2. Editing After Staging
When a file is modified after being staged, Git keeps the staged version and detects the newer modifications separately in the working directory.

This means one file can have both staged and unstaged changes.

## 3. Checking the File State

Run:

```bash
git status
```

The same file may appear under:

- Changes to be committed
- Changes not staged for commit

This indicates that additional modifications were made after staging.

## 4. Comparing the Changes

Compare unstaged changes:

```bash
git diff
```

Compare staged changes with the last commit:

```bash
git diff --staged
```

## 5. Staging the Latest Changes

To include the latest modifications:

```bash
git add index.html
```

Check the result:

```bash
git status
```

The latest changes should now be staged.

## 6. What You Learned
- Editing after staging creates additional unstaged changes.
- Git keeps the staged version separate from newer modifications.
- `git diff` displays unstaged differences.
- `git diff --staged` displays staged differences.
- Running `git add` again stages the latest changes.