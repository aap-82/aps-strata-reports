# aps-strata-samples

A strata-only sample report library for Access Property Services Pty Ltd, deployed to Cloudflare Workers as static assets.

This is a sibling deployment to `aps-reports` — same look-and-feel, but only the two strata samples (no defects sample).

## Layout

```
.
├── wrangler.jsonc          Worker + static-assets config (project name: aps-strata-samples)
└── public/                 Everything served from the worker
    ├── index.html          The strata-only showcase landing page
    ├── aps-logo.svg        Brand mark used in the topbar
    ├── dominic-ogburn.jpg  Portrait for the Meet Dominic section
    ├── strata-report-21-ormond-ashfield.html
    └── strata-report-arlington-grove.html
```

## Deploy

```bash
npx wrangler deploy
```

The Worker will live at `aps-strata-samples.<your-subdomain>.workers.dev`.
