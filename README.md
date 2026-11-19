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


---

## Comparison with Existing Open-Source Projects

Hydro-Glance is described as a water-monitoring and anomaly-detection concept for drought, flood and sea-level signals. These projects provide adjacent hydrology, geospatial and environmental-data foundations rather than exact end-user equivalents.

| Project / resource | Established focus | Relationship to Hydro-Glance |
|---|---|---|
| [pysheds](https://github.com/mdbartos/pysheds) | Watershed delineation and hydrologic terrain analysis from raster data | A focused hydrology analysis library; Hydro-Glance's intended product layer is monitoring multiple water-related indicators and surfacing anomalies. |
| [Hydrofunctions](https://github.com/mroberge/hydrofunctions) | Access and analysis of USGS water-data services | A useful source-integration reference; its geographic/data-source focus is USGS rather than global multi-hazard monitoring. |
| [xarray](https://github.com/pydata/xarray) | N-dimensional labelled scientific datasets and time-series analysis | A general scientific-data foundation for spatiotemporal water observations, not a water-alert application. |

### Where Hydro-Glance is different
- **Multi-hazard framing:** the concept aims to bring drought, flood and sea-level indicators into one monitoring view.
- **Anomaly-to-alert workflow:** its intended value is interpreting time-series changes and surfacing unusual conditions for investigation.
- **Potential regional synthesis:** it could combine sensor, gauge, satellite and model data if each source is documented and harmonized.

### Where established projects are stronger
pysheds and xarray provide mature scientific tooling; Hydrofunctions offers a known water-data integration path. The current Hydro-Glance repository audit found planning/documentation but no executable monitoring, ingestion, modelling or dashboard source.

### Scientific and safety requirements
Define each anomaly in measurable terms, cite source datasets and licences, record units/coordinate systems and missing-data behavior, and evaluate against documented historical events. Clearly separate observations, forecasts and alerts; publish uncertainty and false-alarm/missed-event rates. Do not present an unvalidated prototype as an official flood or drought warning service. This is a concept comparison, not a forecast-accuracy claim.
