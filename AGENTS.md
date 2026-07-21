# Organization Governance Agent Instructions

This repository publishes organization-wide contribution templates and pull request checks. It must never contain product source code, private repository content, credentials, tokens, or secrets.

- Preserve least-privilege GitHub Actions permissions.
- Never use `pull_request_target` to execute pull request code.
- Never add mock or always-success test, lint, or build commands.
- Never add automatic merge behavior or bypass required reviews.
- Treat changes to Issue templates, pull request templates, workflows, and organization rulesets as security-sensitive governance changes.
- Validate YAML and GitHub Actions semantics before publishing changes.
