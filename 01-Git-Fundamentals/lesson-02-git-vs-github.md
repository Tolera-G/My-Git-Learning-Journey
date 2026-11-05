# Lesson 02: Git vs GitHub

## 1. Learning Objectives

By the end of this lesson, you should be able to:

- Explain what Git is.
- Explain what GitHub is.
- Understand the differences between them.
- Describe how they work together.

## 2. What Is Git?

Git is a **distributed version control system** used to track changes in files over time.

It helps developers manage their project history without creating multiple copies of the same project.

With Git, developers can:

- Track changes made to files.
- Save project snapshots called commits.
- Compare different versions.
- Create branches to work on separate features.

**Example:** When developing a website, Git helps you save different stages of your work so you can return to an earlier version if something goes wrong.

## 3. What Is GitHub?

GitHub is an **online platform for hosting Git repositories and collaborating with other developers**.

It allows developers to:

- Store their Git repositories online.
- Share projects with others.
- Collaborate on the same project.
- Review code using pull requests.

GitHub uses Git for version control and provides additional tools for collaboration.

## 4. Git vs GitHub: Main Differences

| Git | GitHub |
|---|---|
| Version control system | Online hosting and collaboration platform |
| Works locally on your computer | Primarily accessed online |
| Tracks project changes | Hosts Git repositories |
| Creates local commits | Shares and displays repository history |
| Manages branches | Supports team collaboration |

**Remember:** Git is the tool that tracks changes, while GitHub is the platform where Git repositories can be hosted and shared.

## 5. How Do They Work Together?

Imagine you are developing a website on your computer.

Git tracks the changes you make and saves them as commits. When you want to share your work online, you push those commits to GitHub.

Three important commands:

```bash
git add .
git commit -m "Add homepage"
git push origin main
```

- `git add .` – Selects changes for the next commit.
- `git commit` – Saves the changes in your local Git repository.
- `git push` – Sends your commits to the remote repository on GitHub.

**Important:** Git can be used without GitHub. You do not need an internet connection to perform normal local Git operations.

## 6. Practice Exercise

Answer these questions to check your understanding:

1. What is Git?
2. What is GitHub?
3. Mention two differences between Git and GitHub.
4. What is the difference between `git commit` and `git push`?

## 7. What You Learned

- Git is a version control system that tracks project changes.
- GitHub is an online platform for hosting Git repositories and collaboration.
- Git and GitHub are different but work well together.
- Commits save changes locally, while pushing sends them to a remote repository.