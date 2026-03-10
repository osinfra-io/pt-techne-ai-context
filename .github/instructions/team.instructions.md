---
applyTo: "**/pt-techne-*/**"
---

# Techne Team Instructions

## Repository Overview

- **`pt-techne-opentofu-workflows`** — Reusable GitHub Actions called workflows for OpenTofu + GCP deployments (OIDC auth, state encryption, job summaries, approval gates)
- **`pt-techne-pre-commit-hooks`** — Pre-commit hooks for IaC validation (`tofu fmt`, `tofu validate`, `tofu test`, docs generation, security scanning)
- **`pt-techne-misc-workflows`** — Reusable called workflows for common automation (build-and-push, Dependabot, Nuclei)
- **`pt-techne-opentofu-codespace`** — GitHub Codespace configuration for standardized IaC developer environments

## GitHub Actions

- All workflow actions must use full 40-character commit SHAs with an inline version comment: `uses: action/name@<sha>  # v1.2.3`
- When consuming `pt-techne-opentofu-workflows` or `pt-techne-misc-workflows`, always reference by full commit SHA with an inline version comment — never by branch or tag
- When modifying workflows, update the Mermaid diagram in `README.md` to reflect the changes

