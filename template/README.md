# Client site template

Starting point for every McNeill Web Design client site. Not published: Netlify only serves the `site/` folder of this repo.

## How to use it

1. Copy `index.html`, `thanks.html` and `netlify.toml` from this folder into the client's new repo (public repo in the `mcneillwebdesign` GitHub organisation).
2. Replace every `{{PLACEHOLDER}}`. Search for `{{` before going live: none should remain.
3. Set the brand colours in the `:root` block at the top of the CSS (main colour, darker shade, accent). Match the client's logo, van or stated preference.
4. Add the client's images next to `index.html`: `hero.jpg`, `about.jpg`, `work-1.jpg` … Compress them first (max ~1600px wide, under ~300KB each).
5. Delete sections the client has no content for: gallery (fewer than 3 photos), reviews (no real reviews), price line on service cards (prices not wanted), hero image (no photo).
6. Extra pages (up to 5 in total) can be made by copying `index.html` and keeping the header/footer.
7. Screenshot at 1280px and 390px wide and fix anything that breaks.

## Rules

- Never invent reviews, ratings, awards, accreditations, years in business or claims the client didn't give.
- Use only photos the client supplied or has the right to use.
- Phone placeholders: `PHONE_DISPLAY` = how it reads (028 9012 3456), `PHONE_TEL` = digits for the link (02890123456), `PHONE_INTL` = +44 format for structured data (+442890123456).
- `SCHEMA_TYPE`: the most specific schema.org type that fits (Electrician, Plumber, HairSalon, Restaurant, AutoRepair … or LocalBusiness).
- `HOURS_SCHEMA` uses schema.org format, e.g. `Mo-Fr 08:00-18:00`. Delete the line if unknown.
- `MAP_QUERY`: URL-encoded town or the address the client is happy to show, e.g. `Lisburn%2C%20Northern%20Ireland`.
- Title tag: `<Trade> in <Main town> | <Business name>`. Meta description: one sentence with the trade, the area and a reason to get in touch (under ~155 characters).
- The contact form is a Netlify form named `contact`. After the first deploy: enable form detection, redeploy, and add an email notification to the client's address.
- The privacy notice assumes no tracking cookies. If analytics or tracking are ever added, add a cookie banner and update the notice.

## Placeholders

BUSINESS_NAME, TRADE, TOWN, AREA, AREA_SHORT, DOMAIN, EMAIL, PHONE_DISPLAY, PHONE_TEL, PHONE_INTL, META_DESCRIPTION, SCHEMA_TYPE, HOURS_SCHEMA, HOURS_DISPLAY, HEADLINE, INTRO, CTA_PRIMARY, POINT_1–3, HERO_ALT, SERVICES_HEADING, SERVICES_INTRO, SERVICE_n, SERVICE_n_TEXT, SERVICE_n_PRICE, ABOUT_1, ABOUT_2, ABOUT_ALT, WORK_n_ALT, REVIEW_n, REVIEW_n_NAME, CONTACT_INTRO, MAP_QUERY.
