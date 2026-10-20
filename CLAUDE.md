# LUNE — website guide

LUNE is a streetwear brand from Nairobi. This repo is the brand website, hosted on Netlify
(auto-deploys on every push to `main`).

## Brand
- Name: LUNE (always uppercase in headings, wide letter-spacing)
- Main tagline: "Made in Motion"
- Drop 01 / first collection: "Lord Knows"
- First product: heavyweight cropped sleeveless tee (boxy fit, dropped armholes, raw hem, small crescent logo on left chest)
- Instagram: https://www.instagram.com/lune.stores
- Voice: short, confident, a little poetic. Night-time, movement, faith. Never salesy.

## Design
- Colours: background #3A2219, deep #2C1912, cream #E8C8B4, copper #C98A70, muted #9C7D70
- Fonts: Cormorant Garamond (headings, italics for taglines), Inter light (body, small caps labels)
- Logo: cream crescent moon with a copper dot, inside thin copper/muted rings (inline SVG in index.html)
- Keep it minimal, lots of space, works perfectly on phones (most visitors come from Instagram)

## Technical
- Plain static site: index.html with inline CSS/JS. No build step, no frameworks unless asked.
- The waitlist uses Netlify Forms (form name "waitlist", data-netlify="true"). Don't break it:
  keep the hidden `form-name` input and the honeypot field.
- Product photos go in /images. Compress them (under ~300KB each) before adding.
- After any change, check the page still looks right on mobile width.
