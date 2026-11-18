# Household Tracker

A free static website for GitHub Pages with Supabase authentication and database storage.

## Deploy
1. Open your empty GitHub repository.
2. Choose **Add file → Upload files** and upload `index.html` (README optional).
3. Commit to `main`.
4. Go to **Settings → Pages**, select **Deploy from a branch**, `main`, `/ (root)`, then save.
5. Open the published Pages URL and sign in with your existing Supabase Auth email and password.

## Important
- Supabase project URL and publishable key are public client configuration. Never add a service-role key, secret key, or database password to this repository.
- Keep RLS enabled. Your account's RLS policies must be configured correctly.
- The first version implements login, monthly dashboard, category breakdown, and transaction add/list/delete. Recurring bills and maintenance screens are placeholders pending verification of the existing database table columns.
- The `transactions` insert assumes columns `user_id`, `transaction_date`, `category_id`, `amount`, and `description`. If the existing table uses different columns, adjust the frontend after reviewing the schema.
- If using GitHub Pages, note that public repositories and published site code are publicly visible; never commit private household financial data.
