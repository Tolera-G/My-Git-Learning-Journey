# Lesson 37: Working with Multiple Remotes

## Learning objectives
- Understand multiple remote repositories.
- Add and inspect remote connections.
- Fetch updates from a specific remote.
- Push changes to the intended remote.

## Core idea
A local Git repository can connect to multiple remote repositories.

Each remote has a name and URL.

## Why it matters
Multiple remotes are useful when collaborating with other developers, contributing to open-source projects, and working with forks.

## How it works

Common remote names:

- `origin`: Usually points to your own remote repository or fork.
- `upstream`: Often points to the original repository from which a fork was created.

These names are conventions, not special Git requirements.

## Practical demonstration

View existing remotes:

```powershell
git remote -v
```

Add another remote:

```powershell
git remote add upstream https://github.com/original-owner/project.git
```

Inspect remotes:

```powershell
git remote show origin
```

Fetch from a specific remote:

```powershell
git fetch upstream
```

Push to a specific remote:

```powershell
git push origin main
```

## Common mistakes and safety notes
- Check remote URLs before pushing.
- Do not confuse `origin` with `upstream`.
- Remote names must be unique.
- Adding a remote does not automatically merge its changes.
- Make sure you have permission to push to the destination repository.

## Practice task
1. Run `git remote -v`.
2. Identify the existing remote names.
3. Inspect the remote using `git remote show origin`.
4. Record whether another remote would be useful.

## Knowledge check
1. What does working with multiple remotes mean?
2. What is the conventional difference between `origin` and `upstream`?
3. Which command adds another remote?
4. How can you fetch updates from the original repository?
5. Why should you check `git remote -v` before pushing?

## What I learned
A local repository can connect to multiple remote repositories. I can use different remote names to fetch and push changes to the correct destinations.
