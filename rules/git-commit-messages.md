# Git Commit Messages

## Description
Conventional commits format for clean git history that works with changelogs and semantic versioning.

## Stack
Any project using Git

## Rule Content
```
Always write git commit messages following the Conventional Commits specification.

Format:
<type>(<scope>): <description>

[optional body]

[optional footer]

Types:
- feat: new feature for the user
- fix: bug fix for the user
- docs: documentation only changes
- style: formatting, missing semicolons (no logic change)
- refactor: code change that neither fixes a bug nor adds a feature
- test: adding or updating tests
- chore: updating build tasks, package manager configs
- perf: performance improvement
- ci: CI configuration changes

Rules:
- Description in lowercase, imperative mood: "add feature" not "added feature"
- No period at the end of description
- Subject line max 72 characters
- Body explains WHY not WHAT
- Breaking changes: add ! after type or BREAKING CHANGE in footer

Examples:
feat(auth): add OAuth2 login with Google
fix(api): handle null response from payment gateway
docs(readme): update installation instructions
refactor(users): extract email validation to utility function
feat!: remove deprecated v1 API endpoints
```
