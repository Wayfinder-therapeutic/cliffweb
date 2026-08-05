# Wayfinder Therapeutic — Website

A warm, welcoming, and inclusive marketing website for **Cliff Stornell, MA** and his
practice, **Wayfinder Therapeutic**. Built as a lightweight static site (plain
HTML, CSS, and a little JavaScript) — no build step, hosts anywhere.

## Pages

| File | Page |
|------|------|
| `index.html` | Home — hero, inclusive statement, "what therapy is like", services preview, narrative-therapy intro, steps, CTA |
| `about.html` | About — Cliff's bio, philosophy, education & credentials |
| `services.html` | Services — individual / couples / group therapy, modalities, formats, fees |
| `faq.html` | FAQ — expandable common questions |
| `contact.html` | Contact — Jane booking button, contact details, message form |

Shared assets: `css/styles.css`, `js/main.js`.

## ✅ Before you go live: fill in the placeholders

Everything that needs your real information is wrapped in **`[SQUARE BRACKETS]`**
so it's easy to find. Search the project for `[` (or use the list below) and
replace each one.

| Placeholder | Where | Replace with |
|-------------|-------|--------------|
| `[PHONE]` | footer (all pages), contact | Your phone / text number |
| `tel:+10000000000` | footer (all pages), contact | Same number in `+1XXXXXXXXXX` format |
| `[EMAIL]` | footer (all pages), contact | Your email address |
| `mailto:hello@example.com` | footer, contact | Same email |
| `[JANE_BOOKING_URL]` | `contact.html` "Schedule on Jane" button | Your Jane URL, e.g. `https://wayfinder.janeapp.com` |
| `[office address]` / `[Office address & details]` | contact, services | Winnipeg office address (or remove if telehealth-only) |
| `[$ rate]` | `services.html` fees | Your session rates |
| `[e.g. Mon–Thu, 10am–6pm]` | contact | Your hours |
| `[ PHOTO OF CLIFF ]` | `about.html` | A real photo (see below) |
| `[Add a warm, personal paragraph…]` | `about.html` | A few personal sentences in Cliff's voice |
| `[Add regulatory body & registration #]` | `about.html` | Registration/licensing details |
| Other `[…]` notes | various | Small confirmations (insurance coverage, modality list, etc.) |

### Adding real photos
The hero, about portrait, and section images currently use tasteful SVG
placeholders. To use real photography, drop images into an `images/` folder and
replace the relevant `<svg …>…</svg>` block (or `.hero-art` / `.split-art` div)
with an `<img src="images/your-photo.jpg" alt="…">`. Warm, natural, welcoming
photos work best — think the reference sites (Orion Wellness, Evergreen).

### Connecting the contact form
The form on `contact.html` currently shows a friendly "email me instead" note on
submit. To make it actually send, point it at a form service — all work with
static hosting:
- **Formspree** — set `<form action="https://formspree.io/f/XXXX" method="POST">`
- **Netlify Forms** — add `netlify` to the `<form>` tag (if hosted on Netlify)
- Or simply delete the form and keep the email/phone/Jane options.

## Running locally
It's static — just open `index.html` in a browser. Or serve it:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying
Works on any static host: **GitHub Pages**, **Netlify**, **Cloudflare Pages**,
**Vercel**, or a traditional web host. For GitHub Pages, enable Pages on this
repo and point it at the branch root.

## Design notes
- **Palette:** Forest & Gold — deep forest green + warm gold/sand on a warm cream
  background. Defined as CSS variables at the top of `css/styles.css`.
- **Fonts:** Fraunces (serif headings) + Nunito Sans (body), via Google Fonts.
- **Tone:** warm, upbeat, welcoming — "wayfinding / finding your path" language,
  strongly inclusive of all genders, relationship styles, and 2SLGBTQIA+ clients.
- Fully responsive with a mobile menu, an accessible FAQ accordion, and a Treaty 1
  land acknowledgement in the footer.
