# Git Workflow Documentation

## Overview
This document describes the version control workflow followed for the **Version Control with Git** project.

## Branching Strategy
- **main** → Stable, production-ready code.
- **dev** → Integration branch where features are tested before moving to main.
- **feature-*** → Short-lived branches for developing new features or changes.

## Steps Followed
1. Initialized the repository locally and connected to GitHub.
2. Created `.gitignore` to avoid tracking unnecessary files.
3. Added `README.md` for project details.
4. Created `dev` and `feature-update-readme` branches.
5. Made changes in `feature-update-readme`, committed, and pushed to GitHub.
6. Created a Pull Request to merge `feature-update-readme` into `dev`.
7. Merged `dev` into `main` after verification.
8. Added Git tag `v1.0` to mark the first stable release.

## Commit Rules
- Use short, descriptive messages.
- Commit often for smaller, trackable changes.

## Pull Request Rules
- Always open a PR from a feature branch to `dev`.
- Review and test before merging into `main`.

## Tags
- Follow semantic versioning: `v1.0`, `v1.1`, etc.
- Tags represent stable milestones.

## .gitignore
- Prevents tracking of:
  - Temporary files
  - Log files
  - Dependency folders (e.g., `node_modules/`)

---
