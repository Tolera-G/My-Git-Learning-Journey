# Lesson 35: Git Authentication

## Learning objectives
- Understand Git authentication.
- Understand HTTPS authentication.
- Explain Personal Access Tokens (PATs).
- Understand SSH key-based authentication.
- Identify the authentication method used by a repository.

## Core idea
Git authentication verifies a user's identity when communicating with remote repositories such as GitHub.

## Why it matters
Authentication protects repositories and ensures that only authorized users can perform restricted operations such as pushing changes.

## Authentication methods

### 1. HTTPS
HTTPS allows Git to communicate securely with GitHub using an HTTPS repository URL.

Example:

```text
https://github.com/USERNAME/REPOSITORY.git
```

Git Credential Manager can handle authentication through browser sign-in and credential storage.

### 2. Personal Access Token (PAT)
A PAT is a secret token used instead of an account password for HTTPS Git authentication.

Common types:
- Fine-grained personal access tokens.
- Classic personal access tokens.

Never expose a PAT in source code or upload it to GitHub.

### 3. SSH
SSH uses a cryptographic key pair:
- Private key: stays on the computer and must remain secret.
- Public key: added to the GitHub account.

Generate an SSH key:

```powershell
ssh-keygen -t ed25519 -C "your-email@example.com"
```

Add the private key to the SSH agent:

```powershell
ssh-add $env:USERPROFILE\.ssh\id_ed25519
```

Test the connection:

```powershell
ssh -T git@github.com
```

## Practical demonstration

Identify the repository's remote URL:

```powershell
git remote -v
```

Check SSH availability:

```powershell
ssh -V
```

HTTPS URLs usually begin with `https://`.

SSH URLs usually begin with `git@github.com:`.

## Common mistakes and security notes
- Never use your GitHub account password as an HTTPS Git password.
- Never share your PAT.
- Never upload your private SSH key.
- Only upload your SSH public key to GitHub.
- Revoke exposed tokens and replace compromised keys.

## Practice task
1. Inspect the remote URL using `git remote -v`.
2. Identify whether it uses HTTPS or SSH.
3. Check whether SSH is available.
4. Record the authentication method currently used.

## Knowledge check
1. What is Git authentication?
2. Why can't you use your normal GitHub password for HTTPS Git operations?
3. What is a PAT?
4. What is the difference between an SSH public key and private key?
5. How can you identify whether a repository uses HTTPS or SSH?

## What I learned
Git authentication verifies my identity when accessing remote repositories. HTTPS can use Git Credential Manager and personal access tokens, while SSH uses a public and private key pair.
