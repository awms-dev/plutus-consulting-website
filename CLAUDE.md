# Plutus Consulting Website

## Project Overview
Single-page marketing website for Plutus Consulting, an AI-powered bookkeeping business targeting sales professionals and small business owners.

- **Domain:** www.plutusconsulting.xyz
- **Live URL:** https://www.plutusconsulting.xyz
- **Repo:** https://github.com/awms-dev/plutus-consulting-website
- **Owner:** Rajat Gogia
- **Entity:** LLC (active)

## Tech Stack
- Static HTML/CSS/JS (single `index.html` file)
- Google Fonts: DM Sans + DM Serif Display
- Formspree for contact form submissions (endpoint: `maqdnabv`)
- Calendly for booking consultations (30-min slot)
- No build tools or frameworks — deploy as-is

## Configuration
One variable at the top of the `<script>` block in `index.html`:

```js
const CALENDLY_URL = 'https://calendly.com/rajatgogia-plutusconsulting/30min';
```

When set, all CTA buttons ("Book a Free Consultation", "Get Started") open Calendly in a new tab. If cleared, they fall back to scrolling to `#contact`.

The contact form POSTs directly to `https://formspree.io/f/maqdnabv` with a `_next` redirect back to the site. No JavaScript involved in form submission.

## Site Structure
- **Nav:** Fixed top nav with blur backdrop, mobile hamburger menu
- **Hero:** Headline, stats (5hrs saved, 24hr turnaround, $0 surprises), dual CTA buttons
- **How It Works:** 3-step cards
- **Services:** 4-card grid (categorization, reconciliation, reporting, CPA-ready)
- **Pricing:** 3 tiers — Essentials ($250), Growth ($450), Premium ($700)
- **Why Plutus:** Value props + benefits panel
- **CTA:** Full-width conversion section
- **Contact:** Description + Formspree-powered form (no email/website displayed)
- **Footer:** Nav links + Privacy Policy modal

## Deployment
- Hosted on **GitHub Pages** from `main` branch
- Custom domain configured via `CNAME` file
- HTTPS enforced, SSL cert auto-provisioned by GitHub
- Every push to `main` auto-deploys

## DNS (Squarespace/Google Domains)
- `www` CNAME → `awms-dev.github.io`
- Nameservers: Google Domains (`ns-cloud-b*.googledomains.com`)
- Apex domain A records for GitHub Pages IPs not yet configured

## Design Tokens
```
Navy:        #1e3a5f (primary brand color)
Sage:        #6b8f71 (success/positive)
Terracotta:  #c4704b (accent/CTA)
Gold:        #d4a843 (logo accent)
Background:  #faf8f5 (warm off-white)
```

## Business Context
- Bookkeeping firm using QuickBooks Online + Booke.ai + AI assistants
- Niche: sales reps, commission-based professionals, solopreneurs
- Growth plan: 1 client → 6 (90 days) → 50+ (3 years)
- See `AI_Bookkeeping_Scaling_Plan.docx` for full business plan
