---
applyTo: "**/pt-techne-*/**"
---

# Techne Team Instructions

## Repository Overview

- **`pt-techne-opentofu-workflows`** — Reusable GitHub Actions called workflows for OpenTofu plan/apply with OIDC auth, state encryption, and job summaries
- **`pt-techne-misc-workflows`** — Additional reusable workflows: container image build-and-push, release automation, dependency updates
- **`pt-techne-pre-commit-hooks`** — Custom pre-commit hooks for IaC validation (tofu fmt, tofu validate, documentation generation)
- **`pt-techne-opentofu-codespace`** — GitHub Codespace definition with pre-installed OpenTofu tooling
- **`pt-techne-development-setup`** — Development environment setup and configuration

## Shared Tooling Considerations

Techne repos provide shared tooling consumed by all other platform teams. Changes can have cross-team impact — all consumers pin to commit SHAs, so releases must be coordinated when breaking changes are introduced.
