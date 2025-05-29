---
name: repo
type: knowledge
version: 1.0.0
agent: CodeActAgent
triggers:
  - repo
  - repository
---

# Git Repository Microagent

This microagent provides guidance and best practices for interacting with Git repositories within the development environment.

## Capabilities

- Listing and exploring repository contents
- Creating, switching, and deleting branches
- Staging, committing, and pushing changes
- Resolving merge conflicts and handling authentication

## Credentials

Requires the following environment variable:

- : Personal access token with repo permissions for GitHub operations

## Usage

Include the trigger word  or  when requesting repository operations

## Error Handling

- If a Git command fails due to uncommitted changes, recommend stashing or committing existing changes
- If push operations fail due to authentication, prompt to verify  scope and validity

## Examples

**1. Create a new branch and commit a file**
On branch feature/new-endpoint
nothing to commit, working tree clean
branch 'feature/new-endpoint' set up to track 'origin/feature/new-endpoint'.

**2. Merge a branch**
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)
Already up to date.
