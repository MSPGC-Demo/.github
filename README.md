# .github

This repo holds the defaults that every repo in the MSPGC-Demo org inherits. GitHub treats a repo named `.github` specially: anything here applies across the org without being copied into each repo.

| Path | What it does |
| --- | --- |
| `profile/README.md` | The public landing page at [github.com/MSPGC-Demo](https://github.com/MSPGC-Demo) |
| `ISSUE_TEMPLATE/` | Issue forms (Bug report, Script request) offered in every repo that has none of its own |
| `PULL_REQUEST_TEMPLATE.md` | The checklist that pre-fills every new pull request |
| `CONTRIBUTING.md`, `SECURITY.md` | Policies linked from every repo's issue and PR pages |
| `workflow-templates/` | Starter workflows listed under **Actions > New workflow** in every repo |
| `.github/workflows/reusable-*.yml` | Shared workflows that other repos call, so the logic lives in one place |

A repo's own file always wins. If `msp-scripts` added its own `CONTRIBUTING.md`, that repo would stop using this one.

For the full walkthrough, see [Org-wide defaults with `.github`](https://github.com/MSPGC-Demo/msp-scripts/blob/main/docs/04-org-defaults.md).
