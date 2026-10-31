# Brickvalue — property, bought and sold

Static marketing site (HTML / CSS / JS, no build step) hosted on GitHub Pages
at `brickvalue.shop`.

> Generated from `C:\Users\souha\coaching-sites-factory` (content file `sites/brickvalue.mjs`).
> To change the content, edit that file and run `node build.mjs brickvalue` — editing the
> HTML here directly would be overwritten on the next build.

## Before you promote this site

| Priority | What | Where |
|---|---|---|
| 🔴 Blocking | Legal page: fill every `[BRACKET]` (legal name, address, state, payment provider). Have a lawyer review it if you can. | `legal.html` |
| 🟠 Important | `contact@brickvalue.shop` doesn't exist yet: set up free email forwarding in Namecheap (*Domain List → Manage → Redirect Email*). | Namecheap |
| 🟠 Important | Contact form: replace `VOTRE_ID_FORMSPREE` with your Formspree id (until then it falls back to `mailto:`). | `contact.html` |
| 🟠 Important | Add a real introduction of the coach (name, background, photo). Never invent credentials. | `about.html` |
| 🟡 Later | Prices ($Stated price / $Negotiated / $Clarified) and plan contents should match what you actually sell. | `index.html` `#pricing` |
| 🟡 Later | Testimonials: only add real ones, with permission. Fake reviews are illegal (FTC). | — |

## Business description (Stripe, directories…)

```
We are Brickvalue, a company based in Schoten in the province of Antwerp, buying and selling residential and non-residential property and land on our own account since 2020. Two Flemish obligations decide what a purchase will really cost you, and both get produced far too late. A building constructed before 2001 cannot be sold in Flanders without an asbestos certificate, which tells you what asbestos-containing material is present and in what condition. And since 2023, buying a home with an energy label of E or F brings a legal obligation to renovate it to label D within five years of the deed — an obligation that transfers to you as the buyer, not to us. Both go in front of you before any offer rather than appearing in the notary's annexes. We sell our own property and we are not an estate agent. Site: brickvalue.shop
```

## Structure

```
index.html            Home: hero, programs, method, pricing, approach, FAQ
programs.html         The four programs in detail
about.html            How we work, principles
contact.html          Contact form
legal.html            Business info, privacy policy, terms of service
404.html              Error page (absolute paths)
assets/css/style.css  Brand colors at the top, shared styles below
assets/js/main.js     Menu, theme, animations, form
```

## DNS (Namecheap → Advanced DNS)

Delete the parking records, then add:

| Type | Host | Value |
|---|---|---|
| A Record | `@` | `185.199.108.153` |
| A Record | `@` | `185.199.109.153` |
| A Record | `@` | `185.199.110.153` |
| A Record | `@` | `185.199.111.153` |
| CNAME Record | `www` | `hamzaniceguy99-glitch.github.io.` |
