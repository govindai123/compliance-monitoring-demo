# Compliance Monitoring — static demo preview

A sanitized, self-contained static preview of the Compliance Monitoring portal UI.
It is hosted on Cloudflare Pages; the GitHub repository is the source of truth.

## What this is

- A single `index.html` with inline CSS and JavaScript.
- All people, SAP numbers, email addresses and circular titles are **fake sample data**.
- No backend, no Excel access, no email sending and no real authentication.
- Login is a local demo: SAP `90000001` / password `Demo1234`.
- State (queries, uploads, read status, changed passwords) is stored only in the
  browser's `localStorage`.

## Deploy / update

From this folder:

```bat
npx.cmd wrangler pages deploy . --project-name=compliance-monitoring-demo
```

Requires `npx.cmd wrangler login` to have been completed once on this machine.
