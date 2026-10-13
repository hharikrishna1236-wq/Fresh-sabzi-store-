# Fresh Sabzi Store

Hindi / Hinglish / English vegetable store with Supabase backend and admin panel.

## Structure
- `index.html` – customer website (products, cart, Cash on Delivery orders)
- `admin.html` – admin panel (open at `/admin.html` or `/admin`)
- `supabase/migrations/` – database schema (already applied to project `fpoqgwhoqkfhrpzavyjy`)
- `supabase/create_admin.sql` – makes your login an administrator

## Deploy
Upload the whole folder (keep `index.html` = customer site, `admin.html` = admin; never rename admin.html to index.html) to Netlify Drop, Vercel or Cloudflare Pages (static, no build step).

## New Supabase project?
1. Run `001_...sql`, then `002_...sql` in the SQL Editor.
2. Replace `SB` (project URL) and `KEY` (publishable key) at the top of the `<script>` in `index.html` and `admin/index.html`.
3. Create the admin user (`create_admin.sql`).

## Security
Only the publishable key is used in the browser. Never put the `service_role` / secret key in these files.

## Not yet built
3 km address validation, UPI verification, order-tracking page, customer login, WhatsApp Business notifications, separate /admin/login routes.
