# TeddyPups U.A.E. — Website Clone

A responsive, multi-page clone of https://puppy.instabizweb.com/ built with plain **HTML, CSS and vanilla JavaScript** (no build step, no framework).

## Pages
| File | Route |
|---|---|
| `index.html` | Home (hero slider, pups grid, two ways, journey, chat mock, trust, families, FAQ, CTA) |
| `puppies.html` | Available puppies with breed + origin filters, "Already gone home" |
| `puppy.html?slug=...` | Puppy detail: gallery/video, facts, steps, enquiry form, prev/next |
| `gone-home.html` | Puppies that found a family |
| `happy-families.html` | Masonry gallery + lightbox + testimonial |
| `how-it-works.html` | Two ways home, promise, delivery, why choose us |
| `faq.html` | Accordion + live search |
| `contact.html` | "Letter" form with validation + WhatsApp hand-off, visit section |

## Structure
```
css/style.css   design tokens, layout, responsive rules
js/data.js      all content (puppies, FAQs, gallery) in one place
js/main.js      shared header/footer, drawer menu, filters, slider,
                lightbox, accordion, form validation, scroll reveal
*.html          page shells
```

## Features
- Fully responsive (mobile drawer menu, sticky WhatsApp/Call bar on phones)
- Hero auto-slider (pauses for `prefers-reduced-motion`), dot navigation
- Breed/origin filters (also via URL: `puppies.html?breed=maltipoo&origin=imported`)
- Puppy detail page driven by `?slug=` from `data.js`
- Lightbox gallery with keyboard (Esc) support
- Accessible accordion, skip link, alt text, focus styles
- Forms: client-side validation, honeypot spam field, then opens WhatsApp with the composed message

## Run locally
```bash
npx serve .          # or: python3 -m http.server 8000
```

## Deploy
Static site — works on Vercel, Netlify, GitHub Pages or Cloudflare Pages (publish directory = repo root, no build command).

## Notes
Images and video are loaded from the reference site's media URLs for this assignment. Replace with your own assets for production use.
