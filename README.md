# VPN Infrastructure Atlas

Interactive public atlas and aggregate infrastructure dataset for analyzing VPN endpoint distribution across countries, ASNs, and hosting networks.

The project provides a static GitHub Pages dashboard and research-oriented aggregate datasets for:

- VPN infrastructure visibility
- ASN and hosting analysis
- VPN/proxy detection research
- fraud and risk feature engineering
- infrastructure concentration analysis
- security and threat-intelligence enrichment

<p align="center">
  <img src="assets/vpn-infrastructure-atlas.jpg" alt="VPN Infrastructure Atlas" width="100%">
</p>

## Live Atlas

https://ipanalytics.github.io/VPN-Infrastructure-Atlas/

## Overview

VPN Infrastructure Atlas visualizes aggregate VPN endpoint footprint across:

- endpoint countries
- ASN/network operators
- hosting providers
- VPN brands/providers

The repository intentionally publishes aggregate infrastructure signals only.

No raw VPN IP lists, credentials, client assets, configuration archives, or private provider data are included.

The dashboard is fully static and runs entirely in the browser using:

- HTML
- JavaScript
- CSV datasets
- GitHub Pages

No backend or database is required.

---

## Features

### Interactive World Map

Explore VPN endpoint distribution by:

- IP count
- `/24` count
- ASN count
- hosting-network concentration

### ASN Explorer

Analyze which ASNs and network operators host the largest observed VPN infrastructure footprint.

### Provider Analysis

Inspect how provider infrastructure is distributed across:

- countries
- hosting providers
- ASNs
- endpoint concentration zones

### Linked Filtering

Provider, ASN, and country filters dynamically constrain each other and persist in the URL.

### CSV Export

Export filtered views directly from the dashboard.

---

## Dataset Scope

Current public snapshot includes:

- VPN-tagged infrastructure only
- aggregate country and ASN statistics
- provider-level infrastructure summaries

The project excludes:

- raw VPN IP feeds
- Tor relay datasets
- open proxy datasets
- customer-derived data
- private provider assets

---

## Data Files

| File | Description |
|---|---|
| `data/provider_country.csv` | Provider footprint grouped by endpoint country |
| `data/provider_asn.csv` | Provider footprint grouped by ASN/network |
| `data/country_summary.csv` | Country-level aggregate statistics |
| `data/asn_summary.csv` | ASN-level aggregate statistics |
| `data/metadata.json` | Snapshot generation metadata |

---

## Use Cases

- VPN/proxy detection research
- IP reputation enrichment
- fraud analytics
- hosting-network analysis
- infrastructure concentration studies
- VPN ecosystem research
- security telemetry enrichment
- abuse and risk modeling

---

## Country Semantics

Country values represent reported or enriched endpoint-location context derived from public metadata and enrichment pipelines.

They should not be interpreted as:

- provider ownership
- legal jurisdiction
- ASN registration country
- company incorporation location

ASN organization names are shown as infrastructure-hosting context only.

---

## Public Dashboard

The GitHub Pages dashboard is designed for:

- infrastructure exploration
- research workflows
- CSV export
- static hosting
- lightweight deployment

The site can be hosted directly from:

- GitHub Pages
- S3/static hosting
- nginx
- Cloudflare Pages

---

## License

Apache-2.0

See `LICENSE`.

---

## Disclaimer

This repository is intended for research, defensive security, fraud prevention, and infrastructure analysis purposes.

All trademarks and provider names belong to their respective owners.
