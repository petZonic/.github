# Contributing to PetZonic

Thank you for your interest in contributing! This guide applies to all repositories in the `@petzonic` organization.

## Getting Started

1. Fork the repository
2. Clone your fork locally
3. Create a feature branch from `develop`
4. Make your changes
5. Open a Pull Request against `develop`

## Branch Naming

| Type | Pattern | Example |
|------|---------|---------|
| Feature | `feature/<short-desc>` | `feature/add-pet-listing` |
| Bugfix | `bugfix/<short-desc>` | `bugfix/fix-login-redirect` |
| Hotfix | `hotfix/<short-desc>` | `hotfix/patch-payment-crash` |
| Chore | `chore/<short-desc>` | `chore/update-deps` |

## Commit Messages

We use [Conventional Commits](https://www.conventionalcommits.org/):

```
type(scope): short description

[optional body]

[optional footer]
```

**Types:** `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`, `ci`, `perf`

**Examples:**
```
feat(api): add pet breed endpoint
fix(web): resolve cart total calculation
docs: update API authentication guide
```

## Pull Requests

- Fill out the PR template completely
- Link the related issue
- Request review from CODEOWNERS
- Ensure CI passes before requesting review
- Squash commits before merge (or use squash-merge)

## Code Standards

- Follow the coding standards in `docs/07-development-guide/coding-standards.md`
- Write tests for new features and bug fixes
- Keep PRs focused — one feature/fix per PR

## Local Development

1. Install prerequisites: Node.js 22.x, pnpm, Docker Desktop
2. Start infrastructure: `cd petzonic-infra && docker compose up -d`
3. Copy `.env.example` → `.env` in the repo you're working on
4. Install dependencies: `pnpm install`
5. Run dev server: `pnpm dev`

## Questions?

Open a Discussion in the relevant repository or reach out to the maintainers.
