# Lesson 27: GitHub Pages

## Learning Objectives
- Understand GitHub Pages.
- Learn how static websites are published.
- Understand branch-based deployment.
- Publish a simple website using GitHub Pages.

## Core Idea
GitHub Pages is a GitHub feature that allows developers to host static websites directly from a GitHub repository.

It supports HTML, CSS, JavaScript, and other static assets.

## Why It Matters
GitHub Pages allows developers to publish portfolios, project websites, and documentation without setting up their own web server.

## How It Works

1. Create website files inside a GitHub repository.
2. Push the files to GitHub.
3. Configure GitHub Pages.
4. GitHub publishes the website.
5. Visitors access it through a web address.

## Publishing Methods

### 1. Deploy from a Branch
GitHub publishes website files from a selected branch and folder.

Example:
- Branch: `main`
- Folder: `/(root)`

### 2. GitHub Actions
GitHub Actions can automate website building and deployment through workflows.

## Practical Demonstration

Create a basic website containing:

```text
my-website/
├── index.html
└── style.css
```

Then:

1. Push the files to GitHub.
2. Open repository Settings.
3. Select Pages.
4. Choose Deploy from a branch.
5. Select `main` and `/(root)`.
6. Save and wait for deployment.
7. Open the published website URL.

## Website URL Format

For a project repository:

```text
https://USERNAME.github.io/REPOSITORY-NAME/
```

## Limitations
GitHub Pages is designed for static websites. It does not directly run custom backend servers such as PHP or Node.js applications.

## Common Mistakes
- Missing `index.html`.
- Incorrect publishing branch or folder.
- Incorrect CSS and image paths.
- Opening the website before deployment finishes.
- Forgetting to push the latest changes.

## Practice Task
Publish a simple HTML and CSS website using GitHub Pages. Open the generated URL and verify that the website works.

## Knowledge Check
1. What is GitHub Pages?
2. Which file commonly serves as the main entry page?
3. What does Deploy from a branch mean?
4. Can GitHub Pages directly run a custom Node.js backend server?

## What I Learned
GitHub Pages makes it possible to publish static websites directly from GitHub repositories. It is useful for portfolios, documentation, and simple project websites.