# Lesson 28: Local vs Remote Repositories

## Learning Objectives
- Understand local repositories.
- Understand remote repositories.
- Identify the differences between them.
- Understand how local and remote repositories communicate.

## Core Idea

A local repository is a Git repository stored on your computer.

A remote repository is a Git repository hosted outside your computer, commonly on platforms such as GitHub.

They are separate copies that can exchange commits and changes.

## Why It Matters

Understanding local and remote repositories is essential for sharing projects, collaborating with developers, and keeping project copies synchronized.

## Local vs Remote

| Local Repository | Remote Repository |
|---|---|
| Stored on your computer | Hosted on a remote server |
| Can work offline | Requires internet to communicate |
| Used for local development | Used for sharing and collaboration |
| Stores Git history | Stores Git history |

## How They Work Together

1. Make changes in your local project.
2. Stage and commit the changes.
3. Push commits to the remote repository.
4. Other developers can access the remote repository.
5. Pull remote changes to update your local repository.

## Important Git Terms

- **Push:** Sends local commits to a remote repository.
- **Pull:** Retrieves and integrates remote changes into a local branch.
- **Local repository:** Your repository on your computer.
- **Remote repository:** A repository hosted elsewhere.

## Practical Demonstration

Inspect the local learning repository:

```powershell
git status
git log --oneline -5
```

Then open the corresponding GitHub repository and compare its commit history.

## Common Mistakes
- Assuming local commits automatically appear on GitHub.
- Assuming GitHub changes automatically appear on your computer.
- Confusing local and remote repositories.
- Forgetting to synchronize changes when collaborating.

## Practice Task
1. Inspect your local repository.
2. Review its recent commit history.
3. Open the corresponding GitHub repository.
4. Compare the commit histories.
5. Identify which repository contains each copy.

## Knowledge Check
1. Where is a local repository stored?
2. What is a remote repository?
3. What does `git push` do?
4. Does creating a local commit automatically update GitHub?

## What I Learned
Local repositories allow developers to work on their computers, while remote repositories allow them to share and collaborate on project history. Git provides operations such as push and pull to exchange changes between them.