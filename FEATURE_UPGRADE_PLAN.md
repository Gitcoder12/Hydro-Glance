# Hydro-Glance — Feature Upgrade Plan

## Objective

A proposed water-monitoring system that would help people notice unusual changes that may indicate flooding, drought or other water-related risks.

## Stage 0 — select problem and data source

- [ ] Choose one water body, station network or dataset.
- [ ] Define intended user and decision supported; do not imply emergency authority.

## P0 — first reproducible data slice

- [ ] Choose a measurable first use case (for example, one public river gauge time series) and identify a lawful public dataset.
- [ ] Define units, sensor/source metadata, timestamps, missing-data semantics and geographic scope.

## P1 — baseline visualization and detection

- [ ] Build an offline time-series ingestion and visualization prototype with historical sample data.
- [ ] Add transparent threshold baseline and compare it to one anomaly-detection method.

## P2 — evaluation and live integration

- [ ] Evaluate lead time, false alarms and missed events on labelled historical periods.
- [ ] Add live data adapters only after source reliability, refresh cadence and outage behavior are documented.

## First milestone acceptance

- [ ] A documented historical dataset can be loaded reproducibly.
- [ ] Timezone, units, missing values and source metadata are handled.
- [ ] Baseline anomaly thresholds are tested on known periods.
- [ ] UI distinguishes observed data from forecasts or risk estimates.
