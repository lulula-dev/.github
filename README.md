# lulula-dev organization governance

This public repository contains contribution templates and deterministic pull request governance for repositories owned by `lulula-dev`. It contains no product source code, credentials, or private repository content.

Organization repositories inherit the Issue and pull request templates when they do not define their own. An organization ruleset requires the central workflow in `.github/workflows/intern-pr-review.yml` for protected default branches.

## Repository contract

Each governed repository must provide real test, lint, and build commands using standard project configuration or these repository-level Actions variables:

- `SETUP_COMMAND` (optional)
- `TEST_COMMAND`
- `LINT_COMMAND`
- `BUILD_COMMAND`

The organization-level `FINAL_REVIEWER` variable identifies the administrator requested after deterministic checks pass. Placeholder commands such as `true` or `exit 0` are prohibited.

Agents and GitHub Actions must never merge pull requests automatically.
Organization-wide contribution templates and pull request governance
