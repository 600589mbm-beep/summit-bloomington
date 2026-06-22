# Summit Auto Care — Bloomington (light theme demo)

A single-file, **light-themed** auto-shop demo site for a Bloomington, MN prospect.
Clean white/zinc base, red-600 accents, Inter type, a seasonal promo bar, and a real
front-end booking flow. Sibling to the dark/premium [summit-auto-care](https://github.com/600589mbm-beep/summit-auto-care)
(Apple Valley) site — different look, same booking UX.

**Live demo:** open `index.html` in any browser (no build step).

## Design
- **Type:** Inter (Google Fonts).
- **Palette:** `zinc-50`/white base, `zinc-900` text, **red-600** accents, emerald for "free".
- **Motion:** IntersectionObserver scroll reveals, hover lifts/shadows; honors `prefers-reduced-motion`.

## Stack
- TailwindCSS (CDN) + vanilla JavaScript. **No build, no backend, one file.**

## Functionality
- Real **3-step booking modal** (service → date/time → details → confirmation), Escape/backdrop close.
  *(Not the `alert()` stub — that was replaced with the full flow.)*
- Sections: promo bar, hero + quick estimate, trust strip, services, tires, offers, reviews,
  shop tips/journal, find-us (hours + map), final CTA, footer, mobile call bar. All nav anchors resolve.

## Customizing per shop
Edit the swap list in the comment at the top of `index.html`: shop name, town, phone
(update **every** `tel:` link), address, founding year, the red promo bar, real reviews +
star count, real coupons, and the Google Maps embed.

> Booking is a front-end demo — wire the final submit to email/Twilio for a live build.
> Never fabricate founding years, reviews, or stats. Address/map are placeholders.
