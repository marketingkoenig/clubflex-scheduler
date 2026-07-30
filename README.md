# ClubFlex Scheduler

This repository contains only the external timer for ClubFlex background jobs.
Application code and credentials are not stored in the repository.

The workflow calls a token-protected production endpoint every five minutes.
The endpoint serializes all work with a database lock and reports failed jobs
back to GitHub Actions.
