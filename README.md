# free-tools-actions

GitHub Actions playground for Kiwi's free-tools stack. Public repo on purpose:
public repos get **unlimited free Actions minutes** on standard runners
(GitHub Free; private repos are 2,000 Linux minutes/month).

Owner: Broooooooke. No card bound, nothing paid.

## Workflows

| Workflow | Trigger | What it does |
|---|---|---|
| `test.yml` | push to `main`, PRs, daily 00:00 UTC, manual | Smoke test: checkout, echo, trivial assert, env sanity |
| `health-check.yml` | daily 08:00 UTC, manual | Public-endpoint health ping (no auth, no secrets) |

## Rules

- Never commit secrets, tokens, UUIDs, passwords, or VLESS links here.
  Sensitive values go in repo Settings → Secrets and variables → Actions.
- No paid runners, no larger runners, no GPU runners.
- If a run ever asks for billing / a card, stop and report — do not upgrade.
