# Lesson 09: Understanding Git Commits

## 1. Learning Objectives
- Understand what a Git commit is.
- Learn how to create commits.
- Understand the purpose of commit messages.
- Verify commit results.

## 2. What Is a Git Commit?
A commit is a saved snapshot of a project's changes at a particular point in time.

Git uses commits to maintain the history of a project.

## 3. Creating a Commit

Use the following command:

```bash
git commit -m "Your commit message"
```

Example:

```bash
git commit -m "Add homepage"
```

- `git commit` creates a commit.
- `-m` allows you to provide a message.
- The message describes the changes.

**Important:** Git commits changes that have been staged.

## 4. What Happens After a Commit?
Git records the staged changes in the local repository's history.

A commit does not automatically upload changes to GitHub.

## 5. Checking the Result

Use:

```bash
git status
```

If there are no pending changes, Git displays:

```text
nothing to commit, working tree clean
```

## 6. Writing Good Commit Messages
Commit messages should clearly describe the changes.

Examples:
- Add homepage
- Fix navigation menu
- Update README instructions

Avoid unclear messages such as `changes`, `update`, or `done`.

## 7. What You Learned
- A commit saves a snapshot of staged changes.
- `git commit` creates a commit.
- `-m` provides a commit message.
- Commits are stored locally.
- Good messages make project history easier to understand.