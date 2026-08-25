# dit-marketing-assets

**PUBLIC** hosting for marketing assets that must be reachable from anywhere —
primarily images referenced inside outbound HTML emails. Files here are served via
`https://raw.githubusercontent.com/thanh-dit/dit-marketing-assets/main/<path>`.

## Rules — read before adding or touching anything

1. **This repo is public by design.** Only put things here that are meant for the open
   internet: email images, logos, public one-pagers. Never data, never documents,
   never anything with a name or an email address in it.
2. **Assets referenced in a sent email are immutable.** An email sitting in someone's
   inbox keeps its URLs forever — renaming, moving or deleting a referenced file breaks
   every copy of every email that ever used it. Once an asset has shipped in an email:
   never rename, never overwrite, never delete.
3. **Version in the filename, don't overwrite** — `dit-hero-play-v1.jpg`, then
   `dit-hero-play-v2.jpg` for the next revision. The old version stays.
4. **Keep files email-sized.** Target < 200KB per image (Gmail clips messages over
   102KB of HTML; images load separately but bloat still hurts).

## Layout

```
email/
  investor/     assets for the investor outreach emails (DIT-Investor-Email-*)
brand/          logos and brand marks, when they need a stable public URL
```

## Current assets

| Path | What | First shipped in |
|---|---|---|
| `email/investor/dit-hero-play-v1.jpg` | Hero for the investor email: purple-cow film thumbnail with play button + "WATCH THE FILM · 2 MIN" baked in (1200×675 @2x for a 600px slot, ~87KB). Regeneration recipe lives in the `dit-investor-outreach` plugin skill (farmer_scraper repo) | DIT-Investor-Email-v5 |
