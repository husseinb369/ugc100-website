# UGC100 Website

## Project
Single-page marketing website for UGC100, an AI-powered UGC operating system.

## Tech
- Single HTML file: `index.html`
- All CSS inline in `<style>` block
- All JS inline in `<script>` block
- Font: Geist (CDN loaded)
- Images: genviral.io R2 CDN (`pub-829011bc778a48a7880c8a27fea4c863.r2.dev`)
- Logo: `logo.png` (1280x1280 chameleon)

## Deploy
```bash
git add index.html && git commit -m "message" && git push && vercel deploy --prod
```
- Vercel project: `ugc100-website`
- GitHub: `husseinb369/ugc100-website`
- Live: https://ugc100-website.vercel.app

## Design Rules
- Light theme (#f7f7f7), green accent (#3d9926)
- Geist font, no em-dashes, no AI-sounding copy
- No "free trial" or "14-day trial" language anywhere
- Dashboard mockups stay dark (#0a0a0a) with glassmorphism
- Buttons: pill-shaped desktop, rounded-xl mobile (match genviral.io)
- Chameleon watermarks: 9% opacity desktop, hidden on mobile
- Always optimize for mobile alongside desktop changes
- Green colored accent words in section headlines

## Clients
- Travly: 40M+ followers, 45+ accounts, travel media
- Gamelancer: 40M+ followers, 54 channels, gaming media
