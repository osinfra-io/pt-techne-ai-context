---
applyTo: "**/pt-techne-*/**"
---

# Techne Team Instructions

## GitHub Actions

All GitHub Actions must use full 40-character commit SHAs with an inline version comment: `uses: action/name@<sha>  # v1.2.3`

Consumers of `pt-techne-opentofu-workflows` and `pt-techne-misc-workflows` reference called workflows by full commit SHA — never by branch or tag.

When modifying workflows, update the Mermaid diagram in `README.md` to reflect the changes.

## Repository Practices

- `pt-techne-opentofu-workflows` — provides `plan-and-apply.yml` and `test.yml` called workflows; includes test workspaces in `tests/` validated in CI via `sandbox.yml`, `non-production.yml`, and `production.yml`
- `pt-techne-misc-workflows` — provides `add-to-project.yml`, `build-and-push.yml`, `dependabot.yml`, `nuclei.yml`, and `release.yml` called workflows consumed across all platform repos
- `pt-techne-pre-commit-hooks` — written in Go; changes require passing `go test ./...`
- `pt-techne-opentofu-codespace` — GitHub Codespace definition; update `.devcontainer/` when tooling versions change

