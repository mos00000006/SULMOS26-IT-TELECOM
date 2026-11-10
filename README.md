# SULMOS26 IT & Telecommunications — Operations Edition v0.2

Deploy the extracted contents to any static HTTPS host (GitHub Pages or Cloudflare Pages). `index.html` must be in the published root directory. Install via browser PWA when supported.

## Operational modules

- Customers, support tickets, field technician jobs, equipment/assets
- Security solutions: CCTV, alarms, access control, intercoms, electric fences, surveys, testing and preventive maintenance dates
- Tech hardware: SKU, categories, prices, stock-on-hand and reorder thresholds
- Hardware sales: draft/confirmed/cancelled sales linked to customer and SKU; confirmation decrements stock; cancellation/change/deletion restores confirmed stock
- LTE and telecom subscriptions: LTE uncapped, LTE capped, 5G, fibre, wireless, network, SIM and router IDs, billing/renewal dates and monthly fees
- Structured cabling: copper/fibre, port counts, metres, technicians and test results
- Live device-record dashboard: open tickets, active contracts, renewals within 30 days, upcoming security servicing and reorder alerts
- Company settings with JSON export and restore

## CRITICAL: storage/security limitations

This release is operational for **single-device, locally saved records** only. It is not a production multi-user SaaS application. `localStorage` data can be lost if browser storage is cleared; export backups regularly. Do not use this version for sensitive records, payment information, customer passwords, SIM PINs or full identity numbers. Password login, tenant/company isolation, cloud synchronization, full accounting, SLA automation, secure file uploads, audit trails, supplier orders, WhatsApp sending, payment collection and automatic billing are NOT provided. Hardware stock is maintained within this browser only, and concurrent multi-user inventory operations are not supported.

## Next production build

Cloudflare Worker API + D1/PostgreSQL, tenant IDs on all business tables, per-company authorization, audit ledger, signed backup/import, and transactional inventory reservations & invoicing. Do not point several browsers at the static PWA and assume they share data.

Official SULMOS26 icon and full logo are included in `assets/`.
