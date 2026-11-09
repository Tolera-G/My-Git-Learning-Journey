# Lesson 31: Pushing Local Changes to GitHub

## Learning objectives
- Understand what pushing means.
- Push local commits to a remote repository.
- Understand the role of `origin` and branch names.
- Configure upstream tracking.

## Core idea
Pushing sends local commits to a remote repository such as GitHub.

## Why it matters
Pushing makes locally committed work available on GitHub so it can be shared, backed up, and used in collaboration.

## How it works
The normal workflow is:

1. Modify files in the working directory.
2. Stage changes using `git add`.
3. Create a commit using `git commit`.
4. Push commits using `git push`.

Git pushes commits, not uncommitted file changes.

## Practical demonstration

```powershell
git status
git branch --show-current
git add README.md
git commit -m "Update README"
git push origin main
```

For the first push when upstream tracking is not configured:

```powershell
git push -u origin main
```

After setting upstream tracking, `git push` is usually sufficient when working on that branch.

## Common mistakes and safety notes
- Check the current branch before pushing.
- Ensure changes are committed first.
- Verify the remote URL using `git remote -v`.
- Do not use force push to bypass an error without understanding its cause.
- You need appropriate access and authentication to push to a repository.

## Practice task
1. Make a small change to README.md.
2. Stage and commit the change.
3. Push the commit to GitHub.
4. Verify the change on GitHub.
5. Check the local repository status.

## Knowledge check
1. What is the difference between `git commit` and `git push`?
2. What does `origin` represent?
3. What is the purpose of `-u`?
4. Can uncommitted changes be pushed?

## What I learned
`git push` transfers local commits to a remote repository. The command connects a local branch to its corresponding remote branch, and upstream tracking can simplify future pushes.
