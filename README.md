# Azan Clock — concept storefront

An art-directed scrolling storefront for the azan wall clocks, in five acts:

1. **Daylight** — an oversized clock cropped by the viewport edge, editorial serif headline.
2. **The day** — a pinned sequence: scrolling drives the clock through Fajr → Isha, the
   active prayer lighting up as the hands sweep.
3. **The clocks** — a horizontal rail of product plates.
4. **What is inside** — a spec table, not icon cards.
5. **The order** — close + order sheet.

Type: Fraunces (display), Plus Jakarta Sans (UI), JetBrains Mono (numbers), Amiri (Arabic).
No frameworks, no build step, no dependencies.

Design questions it answers, deliberately:

- **Light/dark cut between acts.** The night act is the only dark screen, so darkness carries
  meaning instead of being the default mood.
- **Numbers over colour.** Prayer times are tabular mono; the active one is marked by the dot,
  the highlight and the time, so it survives a colourblind eye and a bright screen.
- **Motion with a job.** The scroll drives the clock because the product's job is telling time,
  not because scroll effects are fashionable. `prefers-reduced-motion` collapses the pinned
  sequence into static stacked content.

## Local preview

```bash
python3 -m http.server 8140    # open http://localhost:8140
```

## Note

This is the design concept. The working store with cart, checkout and the owner's Orders panel
lives at https://azan-clock-store.vercel.app

## Live

https://azan-clock-concept.vercel.app
