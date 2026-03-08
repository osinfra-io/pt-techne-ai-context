---
applyTo: "**/pt-techne-*/**"
---

# Techne Team Instructions

## Repository Overview

- **`pt-techne-opentofu-workflows`** — Reusable GitHub Actions called workflows for OpenTofu + GCP deployments (OIDC auth, state encryption, job summaries, approval gates)
- **`pt-techne-pre-commit-hooks`** — Pre-commit hooks for IaC validation (`tofu fmt`, `tofu validate`, `tofu test`, docs generation, security scanning)
- **`pt-techne-misc-workflows`** — Reusable called workflows for common automation (build-and-push, Dependabot, Nuclei)
- **`pt-techne-opentofu-codespace`** — GitHub Codespace configuration for standardized IaC developer environments

### Creating Releases

Tags follow [Semantic Versioning](https://semver.org/): `MAJOR.MINOR.PATCH` — increment MAJOR for breaking changes, MINOR for backwards-compatible additions, PATCH for backwards-compatible fixes.

To release a new version, simply push a new tag to the repository. The tag should be in the format `vX.Y.Z` where `X`, `Y`, and `Z` are integers.

```none
git tag vX.Y.Z
git push origin vX.Y.Z
```
