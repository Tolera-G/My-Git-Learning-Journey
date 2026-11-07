# Lesson 16: Updating the Latest Commit

## Learning objectives
- Understand the purpose of `git commit --amend`.
- Correct the latest commit message.
- Include forgotten files in the latest commit.
- Understand the risks of amending published commits.

## Core idea

`git commit --amend` replaces the latest commit with a new commit containing updated information.

## Common commands

### 1. Change the latest commit message

```bash
git commit --amend -m "New commit message"
```

### 2. Add a forgotten file to the latest commit

```bash
git add filename
git commit --amend --no-edit
```

The `--no-edit` option keeps the existing commit message.

### 3. Inspect the latest commit

```bash
git show --stat HEAD
```

### 4. Check commit history

```bash
git log --oneline -3
```

## How it works

Amending creates a new commit that replaces the previous latest commit in the current branch history. The previous commit object is not directly edited.

## Common mistakes and safety notes

- Amend only the latest commit.
- Check staged changes before amending.
- Avoid amending commits already shared with other people.
- Remember that an amended commit has a different commit ID.

## What I learned

The `git commit --amend` command helps correct the latest commit message or include forgotten changes without creating an additional ordinary commit.