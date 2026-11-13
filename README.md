# Hydro-Glance
Hydro-Glance monitors real-time water anomalies to detect droughts, floods, and sea-level threats before they become disasters.


---

## AI-maintained project notes (secondary — 2026-11-13)

This section supplements the maintainer-authored README above; it does not replace or certify the original claims.

- The current source tree, actual data and executed tests are the implementation source of truth. Roadmap items and draft PRs are not shipped capabilities.
- Preserve real/user-provided data and source provenance. Never replace it with fabricated or synthetic runtime records; isolate and label fixtures.
- Document units, coordinate frames, source, licence, collection date, assumptions, seeds and validation methods where applicable.
- Mark unverifiable fields and metrics as unknown/unverified. Do not invent clinical, scientific or official claims.
- Verify installation, execution and tests against the exact current commit before public use.
- See [MODEL_AUDIT_ROUTER.md](MODEL_AUDIT_ROUTER.md) for independent review instructions.
