# plusone-bot

Daily rotation cron for the FRS Slack +1 reviewer bot.

- `data/reviewers.json` — rotation pool (edit to add/remove people)
- `data/today.json` — today's +1 reviewer (auto-rewritten Mon-Fri by the cron)
- `.github/workflows/daily-rotation.yml` — the cron

The Slack Workflow Builder workflow reads `data/today.json` via raw.githubusercontent.com on each `/plusone` invocation.
