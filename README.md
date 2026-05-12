# Cal YIMBY 2026 Bill Tracker — proof-of-work artifact

Single-page sample of the weekly digest delivered under the productized pilot. Hosted at a public URL to gate cold-email outreach (per `../docs/strategic-review-2026-05-12.md`).

## Contents

- `index.html` — the artifact. Self-contained, no JS, no external assets.

## What this is for

This page replaces a sales call. Cold emails to the 5 Tier-1 YIMBY targets link to this URL as proof of the deliverable. The async-close odds depend on this being live before the first send.

## Hosting (GitHub Pages)

This is a brand-new repo for hosting. The legtracker codebase repo is separate.

Setup steps — run from this directory:

```
cd "C:\Users\nkrum\Documents\Claude\Projects\Legislation Tracker\proof-artifact"
git init
git add .
git commit -m "Initial commit: Cal YIMBY 2026 Bill Tracker sample"
gh repo create cayimby-2026-tracker --public --source=. --push
gh repo edit --enable-pages --pages-branch=main --pages-path=/
```

Or via the GitHub website:
1. Create a new public repo, e.g. `cayimby-2026-tracker`
2. Push this directory's contents
3. Repo Settings → Pages → Source = Deploy from a branch → Branch = `main` / root
4. Live URL will be `https://{username}.github.io/cayimby-2026-tracker/` within 1-2 minutes

## After publishing

1. Verify the URL renders correctly (mobile + desktop).
2. Spot-check 2-3 bill numbers and statuses against [leginfo.legislature.ca.gov](https://leginfo.legislature.ca.gov) — the data was pulled live 2026-05-12 and should still be current within a few days.
3. Update the placeholder `pilot-offer` link inside `index.html` to point to wherever the pilot offer page ends up hosted (or remove the link if you're keeping the offer in the email body only).
4. Update `Nicksresume@protonmail.com` if you want a different contact route surfaced.
5. Once live, add the URL to `../docs/outreach/cold-emails-yimby-top5.md` so every cold email links to it.

## Refresh policy

This is a **sample artifact**, not a live tracker. Pull a fresh OpenStates snapshot and rebuild the page every 2-3 weeks during the outreach window so the data reads as current. After the first paying pilot signs, this page can be retired or replaced with a public marketing site.
