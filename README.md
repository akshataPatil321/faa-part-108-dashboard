# FAA Part 108 Regulatory Dashboard

Metal Raptor's source-linked FAA Part 108 tracker. The public dashboard is deployed with GitHub Pages and refreshed every six hours by GitHub Actions from authoritative sources.

## Update model

- `scripts/update-tracker.mjs` checks the OIRA review record, OIRA meeting docket, and Federal Register API.
- `.github/workflows/update-and-deploy.yml` runs on a six-hour schedule and on demand.
- `docs/data/tracker.json` is the versioned snapshot displayed by the dashboard.
- The browser reloads the most recently published snapshot; it does not scrape regulators directly.

Automated checks identify lifecycle events. Substantive legal and product interpretation remains human-reviewed. Proposed provisions are never described as final mandates.

