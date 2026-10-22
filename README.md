# Football Matchup Dashboard

Generated predictions and performance reports. The model engine, API credentials,
collected database and request cache are kept in a separate private repository.
This repository contains public dashboard output and its deployment workflow.

Website: https://puntman1909-tech.github.io/football-matchup-site/

## One-time Pages activation

Open this repository's Settings → Pages. Under Build and deployment, set Source
to **GitHub Actions**. Then open Actions → Deploy public dashboard → Run workflow.

## Automatic updates

The private engine publishes only index.html, performance.html and .nojekyll.
A fine-grained token scoped only to this public repository with **Contents:
Read and write** is stored as **SITE_PUBLISH_TOKEN** in the private engine's
Actions secrets. No API key or publishing token belongs in this repository.
After successful publication, the push triggers this repository's Pages workflow.

The first dashboard here was recovered from a generated engine report. Data
collection timestamps are shown on the pages. Predictions are research estimates,
remain uncalibrated and are not a guarantee of results.
