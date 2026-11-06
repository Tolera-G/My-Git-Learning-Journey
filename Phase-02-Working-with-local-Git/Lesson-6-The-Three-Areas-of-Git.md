# Lesson 06: Understanding the Three Areas of Git

## 1. Learning Objectives

By the end of this lesson, you should be able to:

- Identify the three main areas of Git.
- Understand the purpose of the working directory.
- Explain what the staging area does.
- Understand how changes become commits.

## 2. The Three Areas of Git

Git uses three main areas to manage changes in a project:

### Working Directory

The working directory is where you create, edit, and delete project files.

Changes made here are detected by Git but are not automatically included in the next commit.

### Staging Area

The staging area is where you select changes that you want to include in your next commit.

The `git add` command moves selected changes into the staging area.

### Git Repository

The Git repository stores the project's committed history.

The `git commit` command records the staged changes as a new commit in the local repository.

## 3. How the Three Areas Work Together

Changes normally move through these areas in the following order:

1. **Working Directory:** Make changes to project files.
2. **Staging Area:** Select changes using `git add`.
3. **Git Repository:** Record changes using `git commit`.

## 4. Important Commands

```bash
git status
git add index.html
git commit -m "Update homepage"
```

- `git status` displays the current state of your repository.
- `git add` stages selected changes.
- `git commit` records staged changes in the local repository.

## 5. What You Learned

- The working directory is where you modify files.
- The staging area holds changes selected for the next commit.
- The Git repository stores committed snapshots.
- `git add` stages changes, while `git commit` records them locally.