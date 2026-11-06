# Lesson 10: Viewing Commit History with git log

## 1. Learning Objectives
- Understand Git commit history.
- View previous commits.
- Identify important commit information.
- Use different `git log` options.

## 2. What Is Git History?
Git history is a record of commits created throughout a project's development.

Each commit records a snapshot and information about the changes.

## 3. The git log Command

To display commit history:

```bash
git log
```

Git displays:
- Commit ID (hash)
- Author
- Date
- Commit message

The newest commit appears first.

## 4. Useful git log Options

### Short History

```bash
git log --oneline
```

Displays each commit in a single line.

### Latest Three Commits

```bash
git log -3
```

Displays the latest three commits.

### Graphical History

```bash
git log --oneline --graph --all
```

Displays a simplified graph of commits and branches.

## 5. What You Learned
- Git records project history through commits.
- `git log` displays commit history.
- `--oneline` provides a shorter view.
- `--graph` displays relationships between commits.