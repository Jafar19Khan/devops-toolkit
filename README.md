# DevOps Toolkit — Git Workflow Project

This repository demonstrates a practical Git and GitHub workflow using:
- `main` for stable releases
- `dev` for integration
- feature branches for independent changes
- pull requests for review and merging
- annotated Git tags for releases

## Branching workflow

```text
main
 └── dev
      ├── feature/docs-and-workflow
      └── feature/git-best-practices
```

## Setup

See `POWERSHELL_GUIDE.md` for the Windows PowerShell instructions.

## Project contents

- `docs/GIT_WORKFLOW.md` — branching and PR workflow
- `docs/COMMANDS_REFERENCE.md` — common Git commands
- `docs/INTERVIEW_QA.md` — Task 4 interview questions and answers
- `.gitignore` — common files excluded from Git
- `.gitattributes` — consistent text-file handling

## Release

After merging the feature PRs into `dev`, merge `dev` into `main` through a GitHub pull request. Then run:

```powershell
.\Complete-Task4.ps1 -Version "v1.0.0"
```
