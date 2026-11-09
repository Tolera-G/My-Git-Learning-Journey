# Lesson 26: Releases and Tags

## Learning Objectives
- Understand Git tags.
- Understand GitHub releases.
- Differentiate between tags and releases.
- Understand version numbering.
- Learn how to create and publish a release.

## Core Idea

A Git tag is a label attached to a specific commit in Git history. It helps identify important versions of a project.

A GitHub release is a published version of a project associated with a Git tag.

## Why It Matters

Releases and tags help developers organize project versions, identify stable points in development, document changes, and distribute software.

## Tag vs Release

| Git Tag | GitHub Release |
|---|---|
| Labels a specific commit | Publishes a project version |
| Exists in Git history | Provides release information |
| Identifies a version | Explains and distributes a version |

## Semantic Versioning

A common version format is `MAJOR.MINOR.PATCH`.

Example: `v1.2.3`

- **Major:** Significant changes that may break compatibility.
- **Minor:** New backward-compatible features.
- **Patch:** Backward-compatible bug fixes.

## Practical Git Commands

Create an annotated tag:

```bash
git tag -a v1.0.0 -m "First stable release"
```

View tags:

```bash
git tag
```

Push a tag:

```bash
git push origin v1.0.0
```

## Creating a GitHub Release

1. Open a GitHub repository.
2. Find the Releases section.
3. Select Create a new release.
4. Choose or create a tag.
5. Select the target branch.
6. Enter a release title.
7. Write release notes.
8. Publish the release.

## Common Mistakes and Safety Notes

- A locally created tag is not automatically pushed to GitHub.
- A tag and a release are not the same thing.
- Use meaningful version numbers.
- Make sure the tag points to the intended commit before publishing.

## Practice Task

1. Open a practice repository.
2. Create a release using tag `v1.0.0`.
3. Add a release title and notes.
4. Publish the release.
5. Verify it in the Releases section.

## Knowledge Check

1. What is a Git tag?
2. What is a GitHub release?
3. What does each part of semantic versioning represent?
4. Which command pushes a specific tag to GitHub?

## What I Learned

Git tags identify important commits, while GitHub releases present project versions with descriptions and downloadable assets. Together, they help developers manage and distribute software versions.