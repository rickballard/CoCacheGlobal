# CoCivia Receipts & Safety (Global)

_Last updated: 20251114T033950Z (UTC seed)_

This page defines how **CoCivia-related work** should leave a trace that is:

- visible to humans and AIs,
- easy to audit later,
- consistent across the CoSuite.

## 1. What counts as a “CoCivia receipt”?

A CoCivia receipt is any short artifact that:

- points at a MegaWave / CoBlock that changed CoCivia state,
- names the repos and branches touched,
- carries at least one stable pointer (PR URL, commit hash, or zip name).

Examples:

- a line in a CoSync note,
- a short `docs/CoCivia/Receipts.md` entry,
- a CoStatus / CoPing focus note (schema owned by Co1).

## 2. Where receipts should live

Minimum expectations:

1. **CoCacheGlobal**

   - `docs/CoCivia/Home.md` is the canonical overview.
   - This `Receipts` page is the *lightweight ledger* of CoCivia-impacting work.
   - Each entry should be one or two bullets with date + pointer.

2. **Other repos (CoAgent, CoSteward, CoCivium, etc.)**

   - May keep their own local notes,
   - but should *also* link back to this global page.

## 3. Entry format (suggested)

Use a simple, append-only list:

- `YYYY-MM-DD — MW_<name> — summary (PR #, branch, or zip name)`

Example:

- `2025-11-14 — MW_CoCiviaHome_v0 — seed home/snippet/positioning (CoCacheGlobal/CoAgent)`

## 4. Ownership + guardrails

- Co1 (CoPrime) owns the **overall receipts pattern** and any future automation.
- This page is only a **seed** pattern and should be kept:

  - short,
  - append-only,
  - free of model-specific chatter.

Future AIs may backfill entries based on CoSync Bus logs and CoPing traces.
