# Lesson 05: Initializing a Git Repository

## 1. Learning Objectives

By the end of this lesson, you should be able to:

- Understand what Git initialization means.
- Use the `git init` command.
- Understand the purpose of the `.git` directory.
- Verify whether a repository has been initialized.

## 2. What Is Git Initialization?

Git initialization is the process of setting up Git inside a project folder so it can manage the project's version history.

Before initialization, a project folder is just an ordinary folder. After initialization, it becomes a Git repository.

## 3. The `git init` Command

The `git init` command initializes a Git repository in the current directory.

```bash
git init
```

When executed, Git creates a hidden directory named `.git` that stores the information needed to manage the repository.

## 4. What Is the `.git` Directory?

The `.git` directory is the internal storage area of a Git repository.

It contains important information such as:

- Commit history.
- Branch information.
- Repository configuration.
- Other internal Git data.

**Note:** Do not manually delete or modify this directory because it contains essential repository information.

## 5. Verifying Initialization

Use the following commands:

```bash
git status
```

This checks whether the current directory is recognized as a Git repository.

On Windows PowerShell, you can also run:

```powershell
dir -Force
```

This displays hidden directories, including `.git`.

## 6. What You Learned

- Git initialization prepares a project folder for version control.
- `git init` initializes a repository.
- Git creates a hidden `.git` directory during initialization.
- `git status` helps verify that Git recognizes the repository.