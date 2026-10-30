# Due Diligence

View-only debt tracker: every card, loan and pay-later plan in one place. It never moves money or pays bills. Installable as a PWA.

Live: https://zephyrprimex.github.io/due-diligence/

- Accounts: email + password sign-up (with email confirmation) via Supabase Auth.
- Data: stored in Supabase Postgres with Row Level Security, so each user can only read and write their own rows.
- The key in `index.html` is Supabase's **publishable** key, which is meant to be public. The secret/service key is never in this repo.
- `vendor/supabase.js` is a local copy of supabase-js v2.118.0 (MIT, see `vendor/supabase-js-LICENSE.txt`), so the app works offline with the service worker.
- Bank linking, email import and screenshot scan are still demo flows that add sample data.
- Privacy policy: `privacy.html` (draft).
