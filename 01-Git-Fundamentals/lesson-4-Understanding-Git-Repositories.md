# Lesson 04: Understanding Git Repositories

## 1. Learning Objectives

By the end of this lesson, you should be able to:

- Explain what a Git repository is.
- Understand the purpose of the `.git` directory.
- Initialize a new Git repository.
- Check whether a folder is a Git repository.

## 2. What Is a Git Repository?

A Git repository is a project directory managed by Git. It contains project files and a hidden `.git` directory that stores information about the repository, including its history and configuration.

A normal folder simply stores files, while a Git repository allows Git to track changes made to those files.

## 3. What Is `git init`?

`git init` is a command used to initialize a new Git repository.

When executed inside a project folder, Git creates a hidden directory named `.git`. This directory stores the information Git needs to manage the project's history.

Command:

```bash
git init
```

## 4. Checking a Git Repository

To check whether your current directory is a Git repository, run:

```bash
git status
```

If Git recognizes the repository, it displays its current status. Otherwise, it reports that the directory is not a Git repository.

## 5. Practical Example

Create a folder and initialize it as a Git repository:

```bash
mkdir git-practice-lab
cd git-practice-lab
git init
git status
```

These commands create a folder, enter it, initialize Git, and check the repository status.

## 6. What You Learned

- A Git repository is a project directory managed by Git.
- The hidden `.git` directory stores important repository information.
- `git init` initializes a new Git repository.
- `git status` displays the current repository status.