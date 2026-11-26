# MatookeSmart Companion MVP

A mobile-friendly prototype based on the MatookeSmart Companion concept proposal. It focuses on useful workflow foundations and deliberately does **not** train or run predictive or image-recognition models.

## Included in this prototype

- Farmer overview with locally recorded price snapshots and practical next steps.
- Market price log with date, location and source fields; a simple descriptive chart is built from recorded observations.
- Early buyer orders and farmer harvest listings, with clear reminders that advance payments are agreements between buyers and farmers—not loans or guaranteed financing.
- Guided, rule-based farm symptom information with uncertainty warnings and extension-worker referrals. No image upload, diagnosis model or treatment prescription is included.
- Sample MatookeSmart Hub product ideas and a processing-trial log that calculates observed input/output yield only.
- Opportunity board for manually posted notices, including source and verification reminders.
- Browser-local persistence using `localStorage`.

## Run locally

Open `index.html` in a modern browser. No package installation, backend, database, external API key or build step is required. Google Fonts are optional; the interface has system fallbacks.

## Important prototype limitations

- Data is stored only in the current browser on the current device. It is not shared across farmers or buyers and is not a production database.
- The buyer orders, price observations and opportunity notices shipped as examples are sample data, not live or verified offers/programmes.
- There is no authentication, payment processing, messaging, escrow, real buyer matching or transaction settlement.
- Price summaries are descriptive averages of the entered records, not future-price predictions or sell recommendations.
- The farm-health flow is general educational decision support, not AI, a diagnosis or a substitute for an agricultural expert.
- Hub product cards are research concepts, not active procurement offers or profitability claims.

## Suggested next engineering steps

1. Validate farmer and buyer workflows with interviews and a small field pilot.
2. Add a backend API and PostgreSQL schema for accounts, farm records, price observations, orders, listings, opportunities and Hub batches.
3. Add authentication, role-based access, consent and secure data handling before collecting real personal data.
4. Add buyer/farmer messaging and order terms, then integrate an appropriately authorised payment partner only after legal review.
5. Replace sample data with clearly sourced field observations. Keep predictive models as a separate later phase after data quality and validation work.

## Files

- `index.html` — app shell and navigation.
- `styles.css` — responsive user interface.
- `app.js` — views, local prototype workflows and local persistence.
