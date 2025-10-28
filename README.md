# GitHub Cron Drift

[![Cron Job](https://github.com/lowlydba/cron-drift/actions/workflows/cron.yml/badge.svg)](https://github.com/lowlydba/cron-drift/actions/workflows/cron.yml)
[![GitHub Cron Drift dashboard](https://img.shields.io/badge/Grafana-GitHub%20Cron%20Drift-orange?logo=grafana&style=flat)](https://lowlysre.grafana.net/public-dashboards/66e12b0c83214d88ab4040521de1e874)
[![Sample Data For Change](https://img.shields.io/badge/Sample%20Data%20For%20Change-%E2%9D%A4-red)](https://sampledataforchange.github.io/)

[![Cron Drift Open Graphic Image](https://github.com/user-attachments/assets/4c9081bf-5284-4f84-afc0-f88e858946cc)][dashboard]

A small observability project for GitHub Actions: a Grafana dashboard and helper tooling that measures "cron drift" — the difference between when a scheduled workflow is supposed to start and when it actually starts on GitHub-hosted runners.

If you use GitHub Actions, you may have noticed scheduled workflows sometimes start late. GitHub warns that the schedule event can be delayed during periods of high load. This project answers the question: how late, how often, and when?

👉 [View the live dashboard][dashboard]

## Why it exists

To stop guessing when scheduled jobs will actually run on GitHub-hosted runners. To help you plan CI/CD and maintenance windows with real data instead of assumptions. To surface daily/hourly patterns and long-tail delays that matter for time-sensitive jobs.

## What you'll see in the dashboard

- Cron drift over time: a time-series of per-run delay (seconds) showing trends over the previous days.
- Quick stats (min, max, mean, median) over a configurable window (e.g., last month).
- Hourly / daily patterns to reveal times when delays spike.
- Recent-run details so you can inspect individual scheduled runs and their delays.

## Contributing

Found a bug, missing feature, or want to improve the dashboard? Open an issue or submit a PR.

[dashboard]: https://lowlysre.grafana.net/public-dashboards/66e12b0c83214d88ab4040521de1e874
