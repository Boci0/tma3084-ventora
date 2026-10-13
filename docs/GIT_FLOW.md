# Git Flow for this project

## Branches

| Branch | Purpose | Created from | Merges into |
|---|---|---|---|
| `main` | Released code only. Every merge gets a version tag. | | |
| `develop` | Where finished features come together. | `main` | |
| `feature/FR-xx-short-name` | One requirement each. | `develop` | `develop` |
| `release/vX.Y.Z` | Final checks before a release. | `develop` | `main` and `develop` |
| `hotfix/short-name` | Urgent fix to a released version. | `main` | `main` and `develop` |

## Daily flow

1. Pick an issue from the Projects board and move it to **In progress**.
2. Make your branch:
   ```bash
   git checkout develop && git pull
   git checkout -b feature/FR-03-login
   ```
3. Commit small and often. Start each message with the FR-ID:
   `FR-03: add login form validation`
4. Push and open a pull request into `develop`. Fill in the template and link the issue (`Closes #12`).
5. Wait for CI to pass and for one teammate to review. The author does not merge their own PR.
6. Merge with **Squash and merge**, then delete the branch.

## Releasing v1.0.0

```bash
git checkout develop && git pull
git checkout -b release/v1.0.0
# bump version in pubspec.yaml, update the user manual, fix last bugs
git checkout main && git merge --no-ff release/v1.0.0
git tag -a v1.0.0 -m "Release v1.0.0"
git push origin main --tags
git checkout develop && git merge --no-ff release/v1.0.0
```

Then create a GitHub Release from the tag and attach the APK and the user manual.

## Settings to turn on in GitHub

**Settings > Branches > Add rule** for both `main` and `develop`:
- Require a pull request before merging
- Require 1 approval
- Require status checks to pass: `Analyze, test, coverage`
- Do not allow bypassing the rules

**Settings > Secrets and variables > Actions:** add `AI_PROXY_URL` (and any other keys). Each person adds their own secrets; do not share them in chat.

## Projects board

Columns: **Backlog, Ready, In progress, In review, Done.**
Milestones: **M1 Proposal, M2 SRS, M3 Design and Implementation, M4 Testing and Release.**
Labels: `feature`, `bug`, `docs`, `must`, `should`, `could`, `ai`.

## Keeping the AI key safe

The Flutter app must not hold the AI provider key. Call a small backend (for example a Firebase Cloud Function) that holds the key and forwards the request. The app only knows the backend URL. This is the "secure API setup" the assessment asks for.

## Rules that are marked

- Meaningful commits (FR-ID plus a clear message), not "update" or "fix".
- Every member opens PRs and reviews other people's PRs. Reviews are part of the individual mark.
- Every AI-assisted change has a LOGAI entry.
