# oss-autopilot

The plans, task boards and daily pipeline behind a portfolio of open-source tools that make AI-era software delivery trustworthy.

| Tool | What it does | Status |
| --- | --- | --- |
| [forge-core](https://github.com/GaganBhayana/forge-core) | Shared engine: GitHub App kit, sandbox runner, LLM layer, evidence core | Building |
| [proof](https://github.com/GaganBhayana/proof) | Verified PR triage: checks whether a PR does what it claims | Building, launch Jan 2027 |
| [bumpfix](https://github.com/GaganBhayana/bumpfix) | Makes failing dependency-upgrade PRs pass, with a public recipe library | Foundation, launch Apr 2027 |
| [flakehound](https://github.com/GaganBhayana/flakehound) | Finds, explains and quarantines flaky tests | Foundation, launch May 2027 |
| [tooltrust](https://github.com/GaganBhayana/tooltrust) | Public A–F trust index for MCP servers and agent skills | Foundation, launch Jul 2027 |
| [harnessci](https://github.com/GaganBhayana/harnessci) | CI for skills, AGENTS.md and MCP configs | Foundation, launch Sep 2027 |

## How the work happens

Built in public with an autonomous pipeline: every day a scheduled Claude session picks tasks from each repo's `docs/TASKS.md`, opens PRs, a second session reviews them, pushes fixes and merges when CI is green. A weekly session refills backlogs and tags releases. The full rules are in [PIPELINE.md](PIPELINE.md); the plan is in [ROADMAP.md](ROADMAP.md); every run is logged in [logs/](logs/).

AI involvement is disclosed on every commit (`Co-Authored-By: Claude`). The owner sets direction and can step in at any time.
