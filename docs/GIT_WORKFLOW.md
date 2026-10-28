# Git and GitHub Workflow

## Branch roles

- `main`: stable, released project history.
- `dev`: integration branch for completed features.
- `feature/*`: short-lived branches for individual changes.

## Pull-request flow

1. Create a feature branch from `dev`.
2. Commit one logical change at a time.
3. Push the feature branch.
4. Open a pull request with base `dev` and compare set to the feature branch.
5. Review the diff and merge using a merge commit.
6. When the release is ready, open a pull request from `dev` to `main`.

## Commit message examples

- `chore: add repository configuration`
- `docs: describe Git branching workflow`
- `docs: add Git command reference and interview answers`

## Release tags

Use annotated tags so the release has a message:

```powershell
git tag -a v1.0.0 -m "Release 1.0.0"
git push origin v1.0.0
```
