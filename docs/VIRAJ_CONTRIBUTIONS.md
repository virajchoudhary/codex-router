# Viraj's upstream contributions

This repository is a fork of
[duolahypercho/codex-router](https://github.com/duolahypercho/codex-router).
Upstream authors own the original router architecture and inherited functionality.
The fork is a contribution workspace, not a router authored entirely by Viraj.

## Inspect merged fixes

| Contribution | What changed | Evidence |
| --- | --- | --- |
| Quota-scope failover | Candidate exclusion follows cooldown scope so independently billed scopes remain eligible; regression coverage checks both directions | [PR 834](https://github.com/duolahypercho/codex-router/pull/834) |
| Subagent lifecycle handling | Lifecycle target deduplication and supported active-namespace selection | [PR 928](https://github.com/duolahypercho/codex-router/pull/928) |
| Route-specific tool-schema compatibility | Reused an existing opt-in repair for a model route and added cycle-edge/control-route regression coverage | [PR 793](https://github.com/duolahypercho/codex-router/pull/793) |

These are attributable merged contributions. They do not establish original
ownership of all router code, a new universal schema engine, live-provider
availability, successful billing routing, or measured throughput.

## Review and run

Use the unchanged [upstream-derived README](../README.md) for installation.
The captured fork's `package.json` reports version `0.6.0`, Node `>=22.19.0`,
`npm run check`, and `npm test`. Fork package version is not the current upstream
release, and the fork's main head does not include every later upstream PR.

The cited PRs are the contribution evidence. Test source and prior test claims
are separate from a fresh suite replay. This portfolio review does not require
configuring any real provider credentials.
