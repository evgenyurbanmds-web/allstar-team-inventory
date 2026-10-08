# All Star Team Inventory

Private inventory and sales management application for All Star Team.

## Architecture
- Frontend: static HTML/JavaScript (prepared separately; not yet deployed).
- Backend: Supabase project `jrqwscixcxpywpzqnayi`.
- Catalog, receipts, sales, refunds, stock balances, audit log and financial reports are stored in Supabase.
- B-Stock is a supplier, not the application brand. Local and other supplier purchases are supported.

## Security / launch checklist
- [ ] Configure owner-only authentication and access to database operations.
- [ ] Verify all database reads and writes through an authorized account.
- [ ] Upload and test the application frontend.
- [ ] Test draft receipts, sales, reversals, weighted-average costing and reports with test data.
- [ ] Publish the frontend at a stable HTTPS URL.

## Important operational rules
- Do not post merchandise into inventory until physically received and explicitly approved by the owner.
- Do not record actual sales, refunds or financial changes without explicit owner confirmation.
- Never commit service-role credentials, passwords, or user financial data to this repository.
- The public Supabase publishable key may be used in the frontend, but it must never bypass row-level security or owner authorization.

## Current state
This repository is not yet a live production website. Backend access restrictions must be completed before using the system for real inventory transactions.
