# Lesson 07: Checking Repository Status with git status

## 1. Learning Objectives

By the end of this lesson, you should be able to:

- Understand the purpose of `git status`.
- Check the current state of a Git repository.
- Identify untracked, modified, and staged files.

## 2. What Is git status?

`git status` is a Git command that displays the current state of a repository.

It helps developers identify files that are new, modified, or staged for the next commit.

## 3. Common File States

- **Untracked:** A new file that Git has not started tracking.
- **Modified:** A previously tracked file that has been changed.
- **Staged:** Changes selected for inclusion in the next commit.

## 4. Using git status

Run the following command inside a Git repository:

```bash
git status
```

Git displays information about the current branch and the state of files in the repository.

## 5. Practical Example

Create a new file and check its status:

```powershell
New-Item -ItemType File -Name "index.html"
git status
```

Git should identify `index.html` as an untracked file.

## 6. What You Learned

- `git status` displays the current state of a repository.
- Git identifies untracked and modified files.
- Staged files are prepared for the next commit.
- Checking repository status helps developers understand their changes before committing.