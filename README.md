# Hydro-Glance
Hydro-Glance monitors real-time water anomalies to detect droughts, floods, and sea-level threats before they become disasters.


## Run status

**No runnable website or application is available in the current default branch.** The repository currently contains project documentation and planning material, but no verified executable frontend, server entry point, or local browser URL. There is nothing to launch in a browser yet; do not use guessed commands or localhost addresses.

When an implementation is added, update this section with its real prerequisites, start command, and browser URL only after verifying it from a clean checkout.


---

## AI-maintained project notes (secondary — 2026-11-13)

This section supplements the maintainer-authored README above; it does not replace or certify the original claims.

- The current source tree, actual data and executed tests are the implementation source of truth. Roadmap items and draft PRs are not shipped capabilities.
- Preserve real/user-provided data and source provenance. Never replace it with fabricated or synthetic runtime records; isolate and label fixtures.
- Document units, coordinate frames, source, licence, collection date, assumptions, seeds and validation methods where applicable.
- Mark unverifiable fields and metrics as unknown/unverified. Do not invent clinical, scientific or official claims.
- Verify installation, execution and tests against the exact current commit before public use.
- See [MODEL_AUDIT_ROUTER.md](MODEL_AUDIT_ROUTER.md) for independent review instructions.

---

## Engineering Audit & Handover — 2026-11-17

**Reviewed commit:** `b0a1e468d2aae5a8dbbb3269f9da80e77318b712` (`main`).

### Confirmed findings
- The reviewed default-branch tree contains project documentation and planning files but no executable monitoring, ingestion, modelling, or dashboard source.
- The README describes real-time water anomaly monitoring for drought, floods, and sea-level threats; those capabilities are not demonstrated by the current source tree.

### Next actions
1. Define the target data sources, spatial/temporal resolution, and measurable anomaly definitions.
2. Implement a reproducible ingestion-to-alert prototype using clearly sourced historical data.
3. Add evaluation against documented ground truth and label forecasts/alerts with uncertainty and limitations.

**Verification status:** source-tree inspection only; no runnable product or automated test suite verified.

---

## Examples Used
- Detecting drought signals from falling reservoir levels
- Identifying flood anomalies after unusually heavy rainfall
- Tracking coastal sea-level changes over time
