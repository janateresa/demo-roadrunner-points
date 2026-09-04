# Roadrunner Rewards — Repetto PTA Demo

A browser-only prototype for a Repetto PTA family engagement and badge system.

## What this version includes

### Family experience
- Demo family login
- Family members (adults + children)
- Family points and Roadrunner levels
- Badge collection
- Upcoming event display
- QR/badge claim flow
- Duplicate badge protection

### PTA admin experience
- Dashboard with family/member/event/badge activity
- Manage Families (demo search)
- Manage Badges
- Create badges with point values and icons
- Create Events
- Automatically create an attendance badge when an event is created
- Automatically generate a unique event QR token
- Activate/deactivate events
- Event QR-code print page

## Try the event flow

1. Open `index.html` in a browser.
2. Click **Admin**.
3. Open **Events**.
4. Create a new event.
5. The event automatically receives an attendance badge and QR token.
6. Open **QR Codes** to see the printable QR cards.
7. Click **My Family → Claim a Badge**.
8. Enter an event token, such as `RR-EVENT-HARVEST-2026`.
9. Choose the family member who attended and unlock the badge.

## Demo data

The demo stores its state in browser `localStorage` under `rr-demo`. No real accounts or backend are connected.

## Next production phase

The prototype is intentionally backend-free. For a real deployment, move authentication, family/member records, badge records, event records, image uploads, QR tokens, and claim history to a secure backend such as Supabase. Add role-based access so only authorized PTA administrators can manage families, badges, and events.
