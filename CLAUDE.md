# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Single-page marketing website for UGC100, an AI-powered UGC operating system that generates, manages, and posts UGC content at scale.

## Architecture

Everything lives in a single `index.html` file — all CSS in an inline `<style>` block, all JS in an inline `<script>` block. No build step, no framework, no dependencies.

- `index.html` — the entire website (~2200 lines)
- `logo.png` — chameleon logo (1280x1280 PNG, transparent background)
- `v2.html` — legacy version, not deployed
- Images hosted on genviral.io R2 CDN: `https://pub-829011bc778a48a7880c8a27fea4c863.r2.dev/hero{N}.webp`

## Deploy

```bash
git add index.html && git commit -m "description" && git push && vercel deploy --prod
```

Vercel project: `ugc100-website` | GitHub: `husseinb369/ugc100-website` | Live: https://ugc100-website.vercel.app

## Design System

- **Theme:** Light (#f7f7f7 background), green accent (#3d9926), Geist font
- **Dashboard mockups:** Always dark (#0a0a0a) with glassmorphism/backdrop-filter — intentional contrast with light page
- **Buttons:** Pill-shaped (border-radius: 100px) on desktop, rounded-xl (12px) on mobile — matches genviral.io style
- **Chameleon watermarks:** 9% opacity with saturate(2) contrast(1.2) on desktop; hidden on mobile (they overflow and look broken)
- **Headlines:** Key words colored green (`color: var(--accent)`)
- **Gradient blobs:** Multiple radial-gradient backgrounds on body for depth (not flat white)

## Content Rules

- **No trial language:** UGC100 does not offer free trials. Never use "14-day trial", "free trial", "try free", etc.
- **No AI slop:** Avoid em-dashes, "empowers", "leveraging", "actionable insights", "game-changer"
- **Keep copy direct and punchy**
- **Always optimize mobile alongside desktop** — viewport is locked (user-scalable=no)

## Key Data

**Clients:**
- **Travly:** 40M+ followers, 2B+ monthly views, 45+ owned accounts. Top: @india 8.3M, @hotels 2M, @destination 2M, @travel 1.4M
- **Gamelancer:** 40M+ followers, 54 channels. Top: @gaming 10.2M, @gamelancer 4.9M, @callofdutygamelancer 1.3M

**Pricing (Self-Service):** Starter $47/mo, Growth $147/mo, Scale $297/mo
**Pricing (Managed Pipeline):** Growth $4,400/mo, Business $8,900/mo, Scale $14,300/mo, Enterprise Custom
