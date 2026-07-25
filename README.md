# Arch Coal (arch-coal)

Arch Coal was a St. Louis-based producer and marketer of metallurgical and thermal coal, renamed **Arch Resources** in 2020. In January 2025 Arch Resources merged with CONSOL Energy in a merger of equals to form **Core Natural Resources, Inc. (NYSE: CNR)**, headquartered in Canonsburg, Pennsylvania. This profile now tracks the surviving company.

**URL:** [https://corenaturalresources.com/](https://corenaturalresources.com/)

**Legacy URL:** [https://archresources.com/](https://archresources.com/) — arch-coal.com no longer resolves.

**Related profile:** [consol-energy](https://github.com/api-evangelist/consol-energy) — the other half of the merger.

## Lineage

| Year | Entity |
|------|--------|
| 1969 | Arch Mineral founded |
| 1997 | Arch Mineral + Ashland Coal merge to form Arch Coal |
| 2020 | Arch Coal renamed Arch Resources |
| 2025 | Arch Resources + CONSOL Energy (est. 1864) merge to form Core Natural Resources |

## Tags:

 - Mining, Coal, Metallurgical Coal, Thermal Coal, Energy, Core Natural Resources, Investor Relations, Fortune 500

## Timestamps

- **Created:** 2026-03-23
- **Modified:** 2026-07-25

## API Surface

**Core Natural Resources does not publish a public developer API.** There is no developer portal, no documented endpoints, and no machine-readable feed published by the company. Its external digital surface is a corporate website plus a separate investor relations portal, both serving HTML and PDF — the investor portal's `/rss`, `/feed`, and `/*/rss` paths were probed on 2026-07-25 and every one returns HTML, not XML. The investor relations portal is therefore listed as a website surface below, **not** as an API.

The only real programmatic access to this company's data is the U.S. Securities and Exchange Commission's own EDGAR APIs, which cover Core Natural Resources under **CIK 0001710366** (the former CONSOL Energy Inc. registrant, renamed in January 2025).

### SEC EDGAR Filings (Core Natural Resources, CIK 1710366)

Third-party government API — filing history as JSON.

- [EDGAR APIs documentation](https://www.sec.gov/search-filings/edgar-application-programming-interfaces)
- [https://data.sec.gov/submissions/CIK0001710366.json](https://data.sec.gov/submissions/CIK0001710366.json)

**Evidence, verified 2026-07-25.** The documentation page describes RESTful JSON APIs on `data.sec.gov` — `https://data.sec.gov/submissions/CIK##########.json` plus the XBRL `companyconcept`, `companyfacts`, and `frames` APIs, no authentication required, with a declared User-Agent and a 10-requests-per-second fair-access ceiling. Calling the endpoint returned HTTP 200 with JSON naming "Core Natural Resources, Inc.", ticker CNR, and the former name "CONSOL Energy Inc." through 2025-01-10.

## Common Properties

- [Website](https://corenaturalresources.com/)
- [Investors](https://corenaturalresources.com/investors/)
- [News & Media](https://corenaturalresources.com/news-media/)
- [Sustainability](https://corenaturalresources.com/sustainability/)
- [Suppliers](https://corenaturalresources.com/suppliers/)
- [Careers](https://corenaturalresources.com/careers/)
- [Contact](https://corenaturalresources.com/contact-us/)
- [LinkedIn](https://www.linkedin.com/company/core-natural-resources)

## Features

| Name | Description |
|------|-------------|
| Metallurgical Coal | Low-Vol (Beckley, Itmann), High-Vol A (Leer, Leer South), and High-Vol B (Mountain Laurel) metallurgical coals for blast furnace steelmaking — roughly 12 million tons annually. |
| High Calorific Value Thermal Coal | High CV thermal coal from the Pennsylvania Mining Complex and West Elk mine for power generation, cement, and industrial use — roughly 30 million tons annually. |
| Powder River Basin Thermal Coal | PRB sub-bituminous coal from Black Thunder and Coal Creek mines in Wyoming. |
| Marine Export Terminals | Ownership stakes in East Coast marine export terminals, with roughly 25 million tons of owned annual export capacity. |
| CONSOL Innovations | Advanced materials and critical mineral extraction research turning coal-based carbon into products for aerospace and other industries. |
| SEC Filings and Investor Reporting | Quarterly earnings, production and sales volume reporting, and SEC filings published through the investor relations portal and EDGAR. |

## Use Cases

| Name | Description |
|------|-------------|
| Investment Research | Analyze Core Natural Resources (NYSE:CNR) financial performance, production volumes, and market position through EDGAR filings and investor materials. |
| Merger and Lineage Tracking | Follow the Arch Coal → Arch Resources → Core Natural Resources lineage, including the CONSOL Energy merger of equals completed January 2025. |
| ESG and Safety Reporting | Access environmental, safety, and governance disclosures published through the corporate sustainability section. |
| Supply Chain and Procurement | Steel producers, utilities, and suppliers reference product specifications, terms and conditions, and the Supplier Code of Conduct. |
| Commodity Market Analysis | Track metallurgical and thermal coal production, export capacity, and sales volumes for commodity market research. |

## Integrations

| Name | Description |
|------|-------------|
| SEC EDGAR | All filings for CIK 0001710366 are available through EDGAR and the SEC's public JSON APIs at data.sec.gov. |
| NYSE | Shares trade on the New York Stock Exchange under the ticker CNR. |

## Artifacts

- [Domain Security](security/arch-coal-domain-security.yml) — live DNS/TLS/HTTP probe of the corenaturalresources.com properties
- [Plans & Pricing](plans/arch-coal-plans-pricing.yml) — records the absence of a commercial API surface
- [Rate Limits](rate-limits/arch-coal-rate-limits.yml) — records the absence of published throttling rules
- [FinOps](finops/arch-coal-finops.yml) — FOCUS-aligned placeholder

> Note: this repo previously carried generated OpenAPI, JSON Schema, JSON-LD, vocabulary, rules, authentication, and agentic-access artifacts describing "investor relations APIs" at `api.archresources.com`. That host does not exist and the company publishes no API, so those artifacts were removed on 2026-07-25.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
