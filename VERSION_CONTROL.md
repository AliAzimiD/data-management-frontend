## **`VERSION_CONTROL.md`**


# Version Control Practices for Data Management Application

This document outlines the version control practices for the Data Management Application. Following these practices ensures a clean and organized codebase, enabling smooth collaboration among developers.

## Branching Strategy

We follow the **Git Flow** branching strategy to manage the project. Below are the main branches:

1. **`main`**:  
   - Contains stable, production-ready code.
2. **`develop`**:  
   - Contains the latest development changes.
   - All feature branches are merged here after code review.
3. **Feature Branches (`feature/<feature-name>`)**:  
   - Used for new features.
   - Naming convention: `feature/<short-description>`
   - Example: `feature/add-user-auth`
4. **Bugfix Branches (`bugfix/<bug-name>`)**:  
   - Used for fixing bugs.
   - Naming convention: `bugfix/<short-description>`
   - Example: `bugfix/fix-login-error`
5. **Release Branches (`release/<version>`)**:  
   - Used for final release preparations.
6. **Hotfix Branches (`hotfix/<version>`)**:  
   - Used for urgent bug fixes in the `main` branch.

## Commit Message Guidelines

We follow the **Conventional Commits** specification to ensure consistent commit messages.

### Commit Types

| Type      | Description                          |
|-----------|--------------------------------------|
| `feat`    | New feature                          |
| `fix`     | Bug fix                              |
| `docs`    | Documentation changes                |
| `style`   | Code style changes (no logic change) |
| `refactor`| Code refactoring                     |
| `test`    | Adding or updating tests             |
| `chore`   | Changes to build tools or dependencies|

### Commit Message Format

```plaintext
<type>(<scope>): <subject>

<body>

<footer>
Example Commit Messages
New Feature:
plaintext
Copy code
feat(api): add endpoint for fetching user data
Bug Fix:
plaintext
Copy code
fix(auth): resolve login error on incorrect credentials
Pull Request (PR) Guidelines
Branch Naming: Ensure your branch follows the naming conventions.
PR Checklist:
Ensure your code is properly formatted.
Ensure all tests pass locally.
Update relevant documentation if necessary.
PR Review:
Assign at least one reviewer for the PR.
Ensure at least one approval before merging.
Merging Strategy:
Use Squash and Merge to keep the commit history clean.
yaml
Copy code

---
