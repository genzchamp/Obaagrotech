# Oba Agrotech Farm Link

**Integrated agricultural support platform for crop and livestock farmers.**

Live project: https://genzchamp.github.io/Obaagrotech/

## What is included

The current front-end MVP brings together five support areas:

1. **Climate and production risks** — an offline decision aid for heat, heavy rainfall, dry spells, flooding and storms, plus a farmer weather-observation log. It does not claim to provide live forecasts.
2. **Trusted agricultural information** — built-in crop, poultry, livestock and general farm-practice guides with search and category filters.
3. **Inputs and support services** — an input-needs checklist and a farmer-managed supplier contact book. Supplier authenticity is not implied.
4. **Farm records and finance readiness** — expense, sales and production records, simple totals and CSV export.
5. **Post-harvest and market access** — harvest planning and a farmer-managed directory for buyers, storage, transport and aggregation contacts.

## Low-connectivity design

- The app has no external JavaScript, font, image or paid API dependency.
- A service worker caches the app shell so it can reopen after a successful first online visit.
- The built-in guides are included in the application and remain searchable offline.
- Farm records are stored in the browser's local storage on the device.
- The farmer can export a CSV backup from the Farm Records section.

**Important:** offline support is not automatic before the first successful load and service-worker installation. Live forecasts, new information, supplier verification, messaging and online marketplace transactions require connectivity and are not yet integrated.

## Data and safety

- Records are stored locally in the current browser/device. They are not synchronised to a server.
- Clearing browser data, using private browsing or changing devices may remove or hide local records. Export backups regularly.
- Supplier, buyer, storage and transport contacts are user-entered, not pre-verified.
- The guides are general educational material, not a substitute for professional agronomic, veterinary, financial or emergency advice.
- No loan approval, live weather feed, payments or verified marketplace transactions are claimed in this MVP.

## Deployment

The project is a static site hosted with GitHub Pages. The root `index.html`, `sw.js`, `manifest.webmanifest` and `icon.svg` are the app files. After a commit reaches the configured Pages branch, allow a short time for GitHub Pages to publish it. Use HTTPS for service-worker and install support.
