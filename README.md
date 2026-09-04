# Roadrunner Rewards — Repetto PTA

A static, working prototype for the Repetto PTA family badge/points system. It is intentionally dependency-free so it can be demoed immediately from GitHub Pages.

## Demo features
- Repetto/Roadrunner branded landing page
- Family sign-in demo
- Family dashboard with points, levels, members, and badge collection
- Badge claiming flow
- Demo QR code for a Harvest Festival badge
- PTA admin dashboard
- Manage families view/search
- Create and activate/deactivate badges
- Automatic QR codes for every badge
- Printable QR-code page
- Demo data persists in browser localStorage

## Run it
You can simply open `index.html` in a browser. For the best experience, publish the folder as a GitHub Pages site.

## GitHub Pages
1. Create a new GitHub repository.
2. Upload `index.html`, `README.md`, and the `assets` folder.
3. In GitHub: Settings → Pages → Deploy from a branch → `main` / root.
4. Open the generated Pages URL.

## Demo paths
- Family: Home → Sign In → My Family
- Admin: Home → Admin → Manage Badges / QR Codes
- Claim: Home → Scan a Badge → enter `RR-HARVEST-2026`

## Production upgrade
This is a **prototype**, not a production system for real family/student data. The next version should move authentication and data to a secure backend such as Supabase, with role-based permissions, server-side QR token validation, duplicate-claim protection, audit logs, password reset, account deletion/export, and privacy controls appropriate for children.

The current UI/data model is intentionally organized around families → members → badges → claims so that migration to a database is straightforward.
