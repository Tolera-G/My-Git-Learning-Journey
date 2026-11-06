# Lesson 03: Installing and Configuring Git

## 1. Learning Objectives

By the end of this lesson, you should be able to:

- Install Git on Windows.
- Verify that Git is installed correctly.
- Configure your Git username and email.
- Check your Git configuration.

## 2. Installing Git

Git must be installed on your computer before you can use its commands.

For Windows users:

1. Visit the official [Git website](https://git-scm.com/install/windows).
2. Download the Windows installer.
3. Run the installer and follow the installation instructions.
4. Keep the recommended default settings unless you have a specific reason to change them.

## 3. Verify Git Installation

After installation, open PowerShell or Git Bash and run:

```bash
git --version
```

This command displays the installed Git version.

Example output:

```text
git version 2.52.0.windows.1
```

If a version number appears, Git is successfully installed and accessible from your terminal.

## 4. Configure Your Git Identity

Git needs to know who is creating commits. We configure a username and email address to identify the author of each commit.

Run these commands:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Replace the example information with your own.

**What does `--global` mean?**

It applies the configuration to all Git repositories belonging to your Windows user account, unless a repository has its own local setting.

## 5. Verify Git Configuration

To check your username:

```bash
git config --global user.name
```

To check your email:

```bash
git config --global user.email
```

To display all global settings:

```bash
git config --global --list
```

Example output:

```text
user.name=Your Name
user.email=your-email@example.com
```

## 6. What You Learned

- Git must be installed before using its commands.
- `git --version` checks the installed Git version.
- `git config` manages Git configuration settings.
- `user.name` and `user.email` identify the author of commits.
- `--global` applies settings across your repositories by default.