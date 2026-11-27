# Runbook

What each alert means and what an operator does about it. Written for someone who did not build
the feature, at the moment something is wrong. A change that adds an alert adds its entry here
(`change-modes` § Definition of Done).

## How to look

- **Health:** `/healthz` answers when the process runs; `/readyz` when it can also reach what it
  needs (the database, for example).
- **Logs:** one JSON object per line, each with a `request_id`; follow one request by its id.
- **Metrics and alerts:** <where they are shown>.

## Alerts

### <Alert name>

- **What it means:** <what is wrong, in the user's terms>.
- **Who is affected:** <which people or which work>.
- **First checks:** <what to look at, in order>.
- **What to do:** <the steps that fix or contain it>.
- **When to escalate:** <to whom, and when>.
