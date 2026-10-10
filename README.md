# Acorn 1.0 public site

This repository hosts only the public, read-only GitHub Pages site for Acorn 1.0. The site files are in `docs/` and the Pages workflow deploys that folder.

The page displays a sanitized market snapshot when one is published. It does not run the bot, dashboard backend, model training, paper trading, or transaction execution. No wallet state, private keys, model artifacts, or trading history belong here.

To refresh market data, run `python pages_export.py` in the bot project, copy the generated `docs/status.json` into this repository, and push the update. The page hides prices when the snapshot is stale.