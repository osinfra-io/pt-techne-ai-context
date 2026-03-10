# pt-techne-ai-context

Techne team-level Copilot instructions for the [osinfra-io](https://github.com/osinfra-io) platform teams workspace.

## Overview

This repository is the **techne team level** of a three-level GitHub Copilot instruction hierarchy. Instructions here apply to all `pt-techne-*` repositories.

```none
Platform   pt-ai-context                   ← universal conventions for all pt-* repos
  └── Team   pt-techne-ai-context          ← this repo (applies to all pt-techne-* repos)
        └── Repo   .github/copilot-instructions.md   ← in every repo (repo-specific only)
```

## What's in this repo

`.github/instructions/team.instructions.md` — loaded via `COPILOT_CUSTOM_INSTRUCTIONS_DIRS`. Contains conventions shared across all techne repositories:

- Reusable called workflows for OpenTofu + GCP deployments and common platform automation
- All GitHub Actions pinned to full 40-character commit SHAs with inline version comments
- Consumers of called workflows reference by full commit SHA — never by branch or tag
- Pre-commit hooks and codespace for standardized IaC development

## Setup

Add this repo alongside `pt-ai-context` in your `COPILOT_CUSTOM_INSTRUCTIONS_DIRS`:

```bash
# ~/.zshrc or ~/.bashrc
export COPILOT_CUSTOM_INSTRUCTIONS_DIRS="\
$HOME/repositories/osinfra-io/platform-teams/pt-ai-context,\
$HOME/repositories/osinfra-io/platform-teams/techne/pt-techne-ai-context"
```
