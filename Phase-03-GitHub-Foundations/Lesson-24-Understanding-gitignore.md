# Lesson 24: Understanding `.gitignore`

## Learning Objectives
- Understand what `.gitignore` is.
- Learn why Git ignores certain files and folders.
- Understand common `.gitignore` patterns.
- Learn how to check whether a file is ignored.

## Core Idea
`.gitignore` is a special text file containing rules that tell Git which untracked files and folders to ignore.

## Why It Matters
It helps keep repositories clean by preventing unnecessary files, temporary files, and sensitive configuration files from being added accidentally.

## Common `.gitignore` Patterns

| Pattern | Purpose |
|---|---|
| `*.log` | Ignore all log files |
| `node_modules/` | Ignore the dependency folder |
| `.env` | Ignore environment configuration |
| `temp.txt` | Ignore a specific file |
| `build/` | Ignore the build folder |
| `!important.log` | Do not ignore this matching file |

## How It Works
Git checks untracked files against the rules in `.gitignore`. Files matching those rules are excluded from normal tracking and staging.

## Practical Demonstration

Example `.gitignore`:

```gitignore
*.log
temp.txt
node_modules/
.env
```

Useful command:

```powershell
git check-ignore -v debug.log
```

This displays the matching ignore rule.

## Important Notes
- `.gitignore` does not delete files.
- It does not automatically stop tracking files already tracked by Git.
- `git rm --cached filename` removes a file from Git's index while keeping the local file.
- Never rely on `.gitignore` alone to protect secrets that have already been pushed.

## Practice Task
1. Create a `.gitignore` file.
2. Add rules for log files and temporary files.
3. Create matching test files.
4. Run `git status`.
5. Use `git check-ignore -v` to inspect an ignored file.
6. Commit the `.gitignore` file.

## Knowledge Check
1. What is the purpose of `.gitignore`?
2. What does `*.log` mean?
3. Where should `.gitignore` usually be placed?
4. Does `.gitignore` stop tracking an already tracked file?

## What I Learned
`.gitignore` helps maintain clean Git repositories by excluding selected untracked files and folders from normal Git tracking.