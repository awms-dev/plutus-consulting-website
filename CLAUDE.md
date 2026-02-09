# Plutus Consulting Website

## Project Overview
Single-page marketing website for Plutus Consulting, an AI-powered bookkeeping business targeting sales professionals and small business owners.

- **Domain:** www.plutusconsulting.xyz
- **Owner:** Rajat Gogia
- **Entity:** LLC (active)

## Tech Stack
- Static HTML/CSS/JS (single `index.html` file)
- Google Fonts: DM Sans + DM Serif Display
- Formspree for contact form submissions
- Calendly for booking consultations (to be configured)
- No build tools or frameworks — deploy as-is

## Configuration
Two variables at the top of the `<script>` block in `index.html` need to be set before going live:

```js
const CALENDLY_URL = ''; // Your Calendly booking link
const FORMSPREE_ID = ''; // Your Formspree form endpoint ID
```

Until `CALENDLY_URL` is set, all CTA buttons scroll to the contact form. Once set, they redirect to Calendly.

Until `FORMSPREE_ID` is set, the contact form will fail to submit. Sign up at https://formspree.io and create a form to get the ID.

## Site Structure
- **Nav:** Fixed top nav with blur backdrop, mobile hamburger menu
- **Hero:** Headline, stats, dual CTA buttons
- **How It Works:** 3-step cards
- **Services:** 4-card grid (categorization, reconciliation, reporting, CPA-ready)
- **Pricing:** 3 tiers — Essentials ($250), Growth ($450), Premium ($700)
- **Why Plutus:** Value props + benefits panel
- **CTA:** Full-width conversion section
- **Contact:** Info + Formspree-powered form
- **Footer:** Nav links + Privacy Policy modal

## Deployment
This is a static site. It can be deployed to any static hosting:
- GitHub Pages (simplest — enable in repo settings)
- Netlify (drag and drop or connect repo)
- Vercel
- Cloudflare Pages

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
