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
  signature/    images in the company email signature, appended by the MCP hub's
                Outlook connector to mail composed through Claude (mcp-hub ADR-013)
brand/          logos and brand marks, when they need a stable public URL
```

## Current assets

| Path | What | First shipped in |
|---|---|---|
| `email/investor/dit-hero-play-v1.jpg` | Hero for the investor email: purple-cow film thumbnail with play button + "WATCH THE FILM · 2 MIN" baked in (1200×675 @2x for a 600px slot, ~87KB). Regeneration recipe lives in the `dit-investor-outreach` plugin skill (farmer_scraper repo) | DIT-Investor-Email-v5 |
| `brand/dit-logo-landscape-transparent-v1.png` | Official landscape logo, transparent background (738×219, ~16KB). Displayed at 186×55 in the email signature | Outlook MCP signature, 2026-09-04 |
| `email/signature/icon-facebook-v1.png` | Facebook icon from the company signature (60×60, shown at 40×40) | Outlook MCP signature, 2026-09-04 |
| `email/signature/icon-instagram-v1.png` | Instagram icon (60×60, shown at 40×40) | Outlook MCP signature, 2026-09-04 |
| `email/signature/icon-twitter-v1.png` | Twitter icon (57×57, shown at 40×40) | Outlook MCP signature, 2026-09-04 |
| `email/signature/icon-linkedin-v1.png` | LinkedIn icon (60×60, shown at 40×40) | Outlook MCP signature, 2026-09-04 |
| `email/signature/icon-youtube-v1.png` | YouTube icon drawn to match the set: red rounded tile, white play button (60×60, shown at 25×25) | Outlook MCP signature, 2026-10-19 |
| `email/signature/neville-banner-v1.png` | "Ask me anything about nutrition" Neville banner (998×198 @2x for a 499px slot, ~112KB) | Outlook MCP signature, 2026-09-04 |
| `email/signature/badge-appstore-v1.png` | Apple's official "Download on the App Store" badge, rasterised from the official SVG (168×56, shown at 84×28) | Outlook MCP signature, 2026-09-04 |
| `email/signature/badge-googleplay-v1.png` | Google's official "Get it on Google Play" badge (478×142, shown at 94×28) | Outlook MCP signature, 2026-09-04 |
