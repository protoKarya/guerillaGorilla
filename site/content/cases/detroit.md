+++
title = "Case Study #1: Detroit Charter Schools"
description = "Cash for Kids 2. 9 convictions. 9 judges. $4.9M/yr public funding. 128+ pages. BLAKE3 braided. The reference implementation."
weight = 10
date = 2026-09-27

[taxonomies]
cases = ["detroit"]
capabilities = ["fear", "prescient", "stride"]
domains = ["legal"]
+++

## Overview

[detroit.primals.eco](https://detroit.primals.eco) is **Case Study #1** — the first non-sporePrint site in the ecoPrimals ecosystem. It documents a Detroit charter school network where a man with 9 criminal convictions runs two schools receiving $4.9M/yr in public education funding.

## The Site as preSCENT

detroit.primals.eco is the **digital instantiation of preSCENT** — ambient presence broadcast through a public evidence library. The site exists. The evidence is public. The record accumulates. Everyone in the network can see it.

## By the Numbers

| Metric | Value |
|--------|-------|
| Criminal convictions | 9 (6 felony, 3 misdemeanor) |
| Annual public funding | $4.9M |
| Revenue to management LLC | 72.67% |
| Math proficiency | 3% |
| Judges with documented connections | 9 across 4 courts |
| Site pages | 128+ |
| Entity nodes | 43 |
| Typed edges | 57 |
| Epistemic levels | 7 |
| Evidence surfaces | 3 (live site + sovereign repo + GitHub mirror) |

## Infrastructure

| Component | Implementation |
|-----------|---------------|
| Static site | Zola + Catppuccin theme + elasticlunr search |
| Entity registries | `config.toml [extra.actors/entities/sources]` |
| Typed edges | `data/edges.toml` with epistemic grammar |
| Content addressing | BLAKE3 `content-manifest.toml` with root hash |
| Sovereign repo | [git.primals.eco/publicRecord/detroit](https://git.primals.eco/publicRecord/detroit) |
| Public mirror | [github.com/defendDetroit/publicRecord](https://github.com/defendDetroit/publicRecord) |
| Build crate | `crates/detroit-build/` (9 modules, 7 build steps) |
| Shared substrate | `crates/litho-core/` (6 modules) |

## Provenance Trio Instantiation

| Layer | Science (original) | Legal (detroit) |
|-------|-------------------|----------------|
| Ephemeral | rhizoCrypt session DAG | fossilRecord epoch archives |
| Certificate | loamSpine RFC 3161 | CASE_REGISTRY typed roles |
| Attribution | sweetGrass PROV-O braids | GRAPH_DATA entity intelligence |

## Verify

- **Live site**: [detroit.primals.eco](https://detroit.primals.eco)
- **Source**: [git.primals.eco/publicRecord/detroit](https://git.primals.eco/publicRecord/detroit)
- **Mirror**: [github.com/defendDetroit/publicRecord](https://github.com/defendDetroit/publicRecord)
- **Sitemap**: [detroit.primals.eco/sitemap.xml](https://detroit.primals.eco/sitemap.xml) — 127 URLs
- **Validation**: [detroit.primals.eco/validate/](https://detroit.primals.eco/validate/)
