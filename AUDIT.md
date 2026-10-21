# Audit Notes — CI Drill Demo

## What this demo shows

- A fresh public repository with a README (default branch: `main`) so there is a clean starting point to work from.
- A GitHub Actions workflow at `.github/workflows/smoke.yml` that triggers on `push`, `pull_request`, and manual `workflow_dispatch`.
- A single job that echoes the marker `SMOKE_DRILL_OK`, making it easy to spot the run succeeding (or failing) in the Actions tab and in the logs.
- A short-lived feature branch (`drill/audit-notes`) carrying this file, opened as a pull request back into `main` — the classic "code change + CI check + review" loop.

## Talking points for the team sync

1. Walk the default branch and point out where the workflow lives.
2. Open the pull request and show how CI attaches a status check to it automatically.
3. Open the Actions run, show the job log line `SMOKE_DRILL_OK`, and show the run's conclusion.
4. Summarize the run in a PR comment so everyone sees how CI results are surfaced where the review happens.

This is a deliberately tiny pipeline — the point is the plumbing, not the payload.
