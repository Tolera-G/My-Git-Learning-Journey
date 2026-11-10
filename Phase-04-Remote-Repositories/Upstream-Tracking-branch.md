# Lesson 34: Upstream Tracking Branches

## Learning objectives
- Understand upstream tracking branches.
- Configure upstream tracking.
- Inspect branch tracking information.
- Understand how upstream tracking simplifies Git commands.

## Core idea
An upstream tracking branch is a remote branch that a local branch follows.

For example, local `main` can track remote-tracking branch `origin/main`.

## Why it matters
Upstream tracking allows Git to remember which remote branch should be used when pushing and pulling.

Instead of repeatedly specifying the remote and branch, you can usually use:

```powershell
git push
git pull
```

## How it works

- `main` is a local branch.
- `origin` is a remote name.
- `origin/main` is a remote-tracking branch.
- Upstream tracking connects a local branch to its corresponding remote-tracking branch.

## Practical demonstration

Configure tracking during a push:

```powershell
git push -u origin main
```

Configure tracking separately:

```powershell
git branch --set-upstream-to=origin/main main
```

Inspect tracking information:

```powershell
git branch -vv
git status -sb
```

## Common mistakes and safety notes
- `origin` and `origin/main` are not the same thing.
- Not every local branch automatically has an upstream.
- Check the current branch before configuring tracking.
- Upstream tracking does not automatically push or pull changes.

## Practice task
1. Run `git branch -vv`.
2. Identify the current local branch.
3. Identify its upstream branch.
4. Run `git status -sb`.
5. Explain the displayed tracking information.

## Knowledge check
1. What is an upstream tracking branch?
2. What does `git push -u origin main` do?
3. What is the difference between `main` and `origin/main`?
4. Why is upstream tracking useful?

## What I learned
Upstream tracking connects a local branch to a remote-tracking branch, making future push and pull operations simpler.
