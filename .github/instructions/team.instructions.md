---
applyTo: "**/pt-techne-*/**"
---

# Techne Team Instructions

## GitHub Actions

All GitHub Actions must use full 40-character commit SHAs with an inline version comment: `uses: action/name@<sha>  # v1.2.3`

Consumers of `pt-techne-opentofu-workflows` and `pt-techne-misc-workflows` reference called workflows by full commit SHA — never by branch or tag.

When modifying workflows, update the Mermaid diagram in `README.md` to reflect the changes.
