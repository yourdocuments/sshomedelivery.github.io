SS HOME DELIVERY — PREMIUM STARTER
===================================

Files
- index.html : customer storefront with search, category filters, sorting, cart, customer details and WhatsApp order handoff.
- admin.html : local demo admin panel to manage products, categories, homepage text, orders and JSON backup.

How to use
1. Extract the ZIP.
2. Open index.html in a browser to preview the storefront.
3. Open admin.html and use demo password: SSHD-Change-Me
4. In Admin Studio, edit products/content. Refresh index.html in the same browser to see updates.

Important limitations
- Admin and storefront share localStorage only when opened from the same browser origin/context. For a reliable shared deployment, host both files on the same domain.
- The demo password is NOT secure production authentication. Do not publish this admin as a secure admin system without server-side authentication and access control.
- WhatsApp ordering opens a prefilled WhatsApp message to the configured number. The customer must press Send in WhatsApp.
- Product photos use remote Unsplash URLs and require an internet connection. Replace with your own licensed product photos before commercial launch.
- Browser-local order records are not a shared database and may not appear on another device. A backend/API is required for production.
