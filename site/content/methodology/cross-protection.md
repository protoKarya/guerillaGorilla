+++
title = "Cross-Protection — Three-Surface Evidence"
description = "Multiple independent surfaces make the record harder to suppress. Every copy is a shield."
weight = 20
date = 2026-09-27

[taxonomies]
capabilities = ["cross-protection"]
domains = ["legal"]
+++

## The Pattern

Every evidence claim in the guerillaGorilla framework exists on at least three independent surfaces:

| Surface | Purpose | Example |
|---------|---------|---------|
| **Live site** | Public access, SEO, human readers | detroit.primals.eco |
| **Sovereign repo** | Git-signed, timestamped, self-hosted | git.primals.eco/publicRecord/detroit |
| **Public mirror** | Independent copy, community access | github.com/defendDetroit/publicRecord |

Suppressing one surface does not affect the others. Taking down the live site leaves the repos. Taking down GitHub leaves the sovereign infrastructure. Seizing the VPS leaves the local gates with full copies.

## BLAKE3 Content Addressing

Every page is BLAKE3 hashed and recorded in `content-manifest.toml`. A single `root_hash` covers the entire content tree. Any modification to any page changes the root hash, making tampering detectable.

The hashes travel with the content. Clone the repo, run `b3sum`, and verify independently. No trust required in any single surface.

## Why Three, Not Two

Two surfaces create a "he said / she said" dispute. Three create **consensus** — if two of three agree, the third is the anomaly. This is the same principle behind Byzantine fault tolerance in distributed systems.

The evidence doesn't need to be trusted. It needs to be **verifiable across independent surfaces**.
