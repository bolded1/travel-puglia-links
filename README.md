# Travel Puglia — Leave a Review

A mobile-first, Linktree-style static page so guests can leave reviews after travelling with [Travel Puglia](https://travelpuglia.com/). Reviews are the primary calls to action; website and social links sit below.

## Review links

Use these exact URLs (do not substitute):

1. **TripAdvisor** — Leave a TripAdvisor review  
   https://www.tripadvisor.com.au/Attraction_Review-g642178-d23733974-Reviews-Travel_Puglia-Ostuni_Province_of_Brindisi_Puglia.html

2. **Google** — Leave a Google review  
   https://www.google.com/maps/place//@40.8092672,17.4424064,14z/data=!3m1!4b1!4m3!3m2!1s0x6ad637e781c5ec9f:0x77f89378ada71966!12e1?entry=ttu&g_ep=EgoyMDI2MDgyNi4wIKXMDSoASAFQAw%3D%3D

3. **Feedback form** — Share your feedback  
   https://form.jotform.com/261118849626869

## Social and site links

- Website: https://travelpuglia.com/
- Instagram: https://www.instagram.com/travelpuglia_
- Facebook: https://www.facebook.com/travelpugliaitalianexperience
- TripAdvisor attraction: https://www.tripadvisor.com/Attraction_Review-g642178-d23733974-Reviews-Travel_Puglia-Ostuni_Province_of_Brindisi_Puglia.html
- Contact page: https://travelpuglia.com/contact/

Footer: Italy +39 320 825 5007 · Australia 1800 836 301 · [info@travelpuglia.com](mailto:info@travelpuglia.com).

## Local preview

Publish directory is `public/` (plain HTML/CSS, no build step).

```bash
# any static server
npx --yes serve public
# or
python3 -m http.server 8080 --directory public
```

## Deploy to Netlify

`netlify.toml` sets `publish = "public"`.

```bash
npx netlify login
npx netlify link          # or create a site
npx netlify deploy --prod --dir=public
```

Git-connected sites will publish `public/` on push. After the first production URL is known, consider making `og:image` and `twitter:image` in `public/index.html` absolute (`https://your-domain/og.jpg`) so social crawlers resolve the 1200×630 card image reliably.

## Brand (from travelpuglia.com)

- Colour: espresso `#2D1A17`, black `#000000`, steel blue `#336699`, backgrounds `#F9F9FA` / `#FFFFFF`, body `#686868`, headings `#2E2E2E`
- Type: Baskervville (headings), Arapey italic (quote-style lede), Roboto (body) via Google Fonts
- Do not use terracotta `#855C5C` or olive — not visible on the live site

## Assets

| File | Role |
| --- | --- |
| `public/logo.png` | Official 1187×192 wordmark |
| `public/og.jpg` | 1200×630 Puglia door crop (Open Graph + page hero) |
| `public/favicon.svg` | Brand-dot favicon derived from the logo |
