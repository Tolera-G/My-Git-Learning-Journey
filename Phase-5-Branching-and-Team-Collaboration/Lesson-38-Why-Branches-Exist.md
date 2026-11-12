# Lesson 38: Why Branches Exist

## Learning Objectives

- Understand what Git branches are.
- Explain why developers use branches.
- Understand the purpose of the `main` branch.
- Recognize how branches support teamwork.

## Core Idea

A Git branch is a separate line of development within a repository. It allows developers to work on features, fixes, or experiments without directly changing the main development line.

## Why Branches Matter

Branches help developers:

- **Isolate work:** Develop features independently.
- **Reduce risk:** Avoid disturbing stable work.
- **Collaborate:** Allow multiple developers to work separately.
- **Organize changes:** Keep different tasks separated.
- **Review work:** Inspect changes before integrating them.

## Understanding Main

`main` is a commonly used name for a repository's primary branch. It is a convention, not a branch name required by Git.

Other repositories may use names such as `master`.

## Practical Commands

```bash
git branch
git branch --show-current
git branch -a
```

| Command | Purpose |
|---|---|
| `git branch` | Lists local branches |
| `git branch --show-current` | Shows the current branch |
| `git branch -a` | Lists local and remote-tracking branches |

## Important Notes

- A branch provides a separate line of development.
- Changes made on one branch do not automatically appear on another.
- Branches can later be integrated using merging.
- Branches make collaboration and experimentation safer.

## Practice Task

1. Open your Git practice repository.
2. Run `git status`.
3. Run `git branch`.
4. Run `git branch --show-current`.
5. Run `git branch -a`.
6. Observe the results and identify your current branch.

## What I Learned

Git branches allow developers to work independently without directly disturbing the main development line. They make software development safer, more organized, and easier to manage as a team.