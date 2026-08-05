# Platforms by Isaiah Goodrich

Marketing site for custom website builds — creators and small businesses.

Single-file static site. No build step, no dependencies.

- `index.html` — the entire site (markup, CSS, JS inline)
- `images/mandi-phone.jpg` — photo used in the hero phone mockup and the Live Work card
- `vercel.json` — headers + clean URLs

## Run locally

Open `index.html` in a browser, or:

```
python3 -m http.server 8000
```

## Structure

1. **Intro** — canvas particle animation assembles "PLATFORMS BY / Isaiah Goodrich", holds,
   then scatters. Skips on Esc or the Skip button, and force-dismisses after 7s no matter what.
   Respects `prefers-reduced-motion`.
2. **Hero** — headline + phone mockup rendering a miniature of mandibagley.com, with two
   floating status cards.
3. **The Build** — 01–04 feature blocks.
4. **Who It's For** — creators / small businesses.
5. **Process** — three steps.
6. **Live Work** — Mandi Bagley card + two open slots for sites still to come.
7. **Contact** — form that composes a prefilled `mailto:` to isaiahgoodrch@gmail.com.

## Notes

- The contact form has no backend. Submitting builds a `mailto:` link and opens the
  visitor's mail app. To collect submissions server-side instead, point the `<form>` at a
  Formspree/Basin endpoint and delete the submit handler at the bottom of `index.html`.
- Deliberately **no analytics** — none is offered or mentioned anywhere on the page.
- Contact email is `isaiahgoodrch@gmail.com` (appears in the form handler, the contact
  sidebar, and the footer).
