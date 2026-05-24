# PermitCore — public API documentation

Source for **docs.permitcore.io**, built on [Mintlify](https://mintlify.com).

## Local preview

```bash
npm i -g mintlify
mintlify dev
```

Opens at `http://localhost:3000`.

## Editing

- All pages are `.mdx` files at the repo root or under `concepts/` / `api-reference/`
- Navigation order lives in `mint.json` → `navigation`
- Brand tokens (colors, fonts, logo) live in `mint.json` → `colors`, `font`, `logo`

## Deploy

Mintlify auto-deploys on push to `main`. After connecting this repo in
the Mintlify dashboard, pushing here ships to `docs.permitcore.io`.

## Founder action items (one-time setup)

1. Connect this repo in <https://dashboard.mintlify.com>
2. Add CNAME record: `docs.permitcore.io` → `cname.mintlify.app` (or whatever
   Mintlify provides in the dashboard's domain settings UI)
3. Replace `phc_REPLACE_WITH_NEXT_PUBLIC_POSTHOG_KEY_FROM_VERCEL` in
   `mint.json` `analytics.posthog.apiKey` with the actual `NEXT_PUBLIC_POSTHOG_KEY`
   value from the permitcore-site Vercel env (paste, commit, push)

## Visual audit

The cross-ref / launch audit doc lives in the main site repo:

`permitcore-site/docs/audits/visual-audit-b1.6-docs-site-2026-05-24/`

That doc captures both the docs site visuals AND the main site
cross-reference updates (nav, footer, /docs redirect) in one place.
