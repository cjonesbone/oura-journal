# Oura Journal Sync

A personal, single-user tool that pulls sleep, readiness, and recovery data from the
[Oura Cloud API](https://cloud.ouraring.com/docs) (v2) and writes it into a local daily
health journal (an Obsidian vault) on the owner's machine.

## What it does

- One-time setup: register a personal OAuth application pointing at
  `http://localhost:8788/callback`, then run a small local helper to grant access.
- A scheduled local job fills the "Oura" section of each daily journal entry from the
  most recently completed night (readiness score, sleep score, total sleep, resting
  heart rate, HRV, respiratory rate, and body-temperature deviation).
- OAuth tokens are stored locally and auto-refreshed, so no re-auth is needed day to day.
- Everything runs and stays on the owner's own machine.

Related pages: [Terms of Service](TERMS.md) · [Privacy Policy](PRIVACY.md)
