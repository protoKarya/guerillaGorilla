+++
title = "The Dispersal Pattern — Primal-as-Site"
description = "Any domain that produces typed, citable claims can produce a .primals.eco site. The substrate is domain-agnostic."
weight = 30
date = 2026-09-27

[taxonomies]
domains = ["legal", "science"]
+++

## The Pattern

detroit.primals.eco proved that the ecoPrimals infrastructure substrate generalizes beyond science. Any domain that produces **typed, citable claims with verifiable sources** can produce a `.primals.eco` static site using the shared litho-core substrate.

## Architecture

```
sporePrint Catalogue (config.toml entity_registry, sources.toml)
        │
        ▼
site.primals.eco (Zola static site)
  ├── config.toml (typed registries — actors, entities, sources)
  ├── content/*.md (pages with TOML front matter)
  ├── data/edges.toml (typed edges with epistemic grammar)
  └── crates/site-build/ (uses litho-core)
        │
        ▼
content-manifest.toml    graph.json         braids.json
(BLAKE3 hashes)          (typed edges)      (PROV-O attribution)
        │                     │                   │
        ▼                     ▼                   ▼
  nestGate CAS         sweetGrass braids    loamSpine spine
```

## Pattern Components

1. **Zola Site with Entity Registries** — typed registries in `config.toml [extra.*]`
2. **Typed Edges with Epistemic Grammar** — 7 levels from `record` to `adjudicated`
3. **Build Crate using litho-core** — 6 shared modules (frontmatter, manifest, graph, report, registry, provenance)
4. **Provenance Trio Wiring** — build output feeds nestGate + sweetGrass + loamSpine
5. **Convergence Depth Meter** — 5 levels: CAS → DAG → Spine → Braid → Signed witness

## Hierarchy

```
gorilla.primals.eco (methodology — you are here)
    └── detroit.primals.eco (Case Study #1 — Banks enterprise)
    └── [future].primals.eco (Case Study #N)

sporeprint.primals.eco (ecosystem catalogue — parent)
    └── gorilla.primals.eco (registered methodology)
    └── detroit.primals.eco (registered case study)
```

## Who Can Adopt This

| Domain | Registry types | Edge grammar |
|--------|---------------|-------------|
| **Legal (active)** | actors, entities, sources | 7 epistemic levels |
| **Methodology (active)** | capabilities, cases, tools | operational levels |
| **Science (future)** | researchers, papers, datasets | validation levels |
| **Medical (future)** | protocols, trials, outcomes | evidence grades |

The substrate is domain-agnostic. Each site owns its registries and edge grammar; litho-core provides the common plumbing.
