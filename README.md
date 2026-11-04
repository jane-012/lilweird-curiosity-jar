# LilWeird After Dark Game Hub — Prototype

## Files
- `index.html`: Game Hub landing page.
- `curiosity-jar.html`: unmodified copy of the uploaded Curiosity Jar application.
- `pick-your-poison.html`: new playable, local-browser prototype.

## Deploy to GitHub Pages
1. On `feature/game-hub`, place all three HTML files in the repository root.
2. Preview the branch locally or through a temporary deployment. GitHub Pages normally serves the configured publication branch, so avoid switching Pages to this branch until tested.
3. When ready, merge into `main` after checking Curiosity Jar still works and the Supabase credentials can be entered.

## Important limitations
- Pick Your Poison does **not** yet connect to Supabase or support two-device multiplayer.
- Both votes are recorded on one device; the first vote is hidden in the UI but this is not a secure voting mechanism.
- Pick Your Poison cards are saved in `localStorage` only. Export JSON backups regularly.
- The Curiosity Jar HTML is preserved unchanged. It still uses the existing Supabase project and database functions.
- No database migrations or RLS policies are included in this prototype. Those require confirming the actual Supabase schema and desired shared-room permissions.
- A GitHub branch protects source code, **not** the Supabase database. Export database tables separately.
