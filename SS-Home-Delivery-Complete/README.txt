# SS Home Delivery Service — Complete Starter ZIP

## Included
- `index.html` — Bengali storefront, responsive layout, product search/category filtering, wishlist, cart, and WhatsApp checkout.
- `admin.html` — browser-based demo admin panel for products, categories, homepage text, contact settings, and JSON backup/restore.

## Run locally
1. Extract the ZIP.
2. Open `index.html` in your browser.
3. Open `admin.html` to manage the storefront.
4. Demo password: `SSHD-Change-Me` (change it in `admin.html` for private demos).

## Important current limitation
This is a **browser-only prototype**. Content is saved to that browser's `localStorage`; it does not sync to other browsers, devices, or customers. The demo password is visible in client-side source and is **not secure authentication**. Do not use this admin gate to protect real customer data or a production business.

The current checkout sends the cart through WhatsApp and does not create a server-side order record. Admin's Orders section explains this limitation.

## Planned Cloudflare production upgrade
After the domain is purchased, deploy the public storefront and admin UI with Cloudflare Pages (or Workers Static Assets), then connect a Cloudflare Worker API and D1 database. Implement server-side authentication/authorization, sessions, input validation, rate limiting, order records, product/category/settings tables, and safe image storage (e.g. R2). Never put API secrets in HTML. Only after that upgrade will changes made by an authorized admin be visible to all visitors and devices.

## Data notes
- Storefront and admin use the same `sshd_` localStorage keys when opened in the same browser/origin.
- If opening the two files via `file://`, browser storage behavior can vary. For reliable local testing, use a simple local static server or deploy to a preview URL.
- Export JSON backups from Admin → Backup & setup before testing resets/imports.
