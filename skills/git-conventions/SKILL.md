---
name: "git-conventions"
description: "Git commit message and branching conventions. Use when the user asks to write a commit message, create a branch, or review git history. Also activate when the conversation involves conventional commits, semantic versioning, or branch naming patterns."
---

# Git Conventions

Standard git workflow conventions for consistent commit messages and branch naming.

## Commit Messages

Use conventional commits format:

```
<type>(<scope>): <subject>
```

### Types

| Type | Use for |
|------|--------|
| `feat` | New features |
| `fix` | Bug fixes |
| `docs` | Documentation changes |
| `refactor` | Code restructuring without behavior change |
| `test` | Adding or updating tests |
| `chore` | Build, tooling, dependency updates |

### Rules

- Subject line max 72 characters
- Use imperative mood ("add" not "added")
- No period at the end
- Scope is optional but encouraged

## Branch Naming

```
<type>/<short-description>
```

Examples: `feat/user-export`, `fix/login-redirect`, `docs/api-reference`

## Versioning

Follow semver: `MAJOR.MINOR.PATCH`

- `feat` → bump MINOR
- `fix` → bump PATCH
- Breaking changes → bump MAJOR (add `BREAKING CHANGE:` footer)
