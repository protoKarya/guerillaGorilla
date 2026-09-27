+++
title = "Verify"
description = "Clone the repos. Check the hashes. Reproduce the claims. Trust nothing — verify everything."
template = "section.html"
+++

## Verify This Site

```bash
# Clone the source
git clone https://github.com/protoKarya/guerillaGorilla.git
cd guerillaGorilla

# Build locally
cd site && zola build

# Compare with live site
curl -s https://gorilla.primals.eco/sitemap.xml | grep '<loc>'
```

## Verify Detroit (Case Study #1)

```bash
# Clone the evidence repository
git clone https://git.primals.eco/publicRecord/detroit.git
cd detroit

# Verify content integrity
b3sum site/content/**/*.md
# Compare with content-manifest.toml root_hash

# Build locally
cd site && zola build
```

## Verify the Ecosystem

```bash
# Clone sporePrint (the catalogue)
git clone https://github.com/ecoPrimals/sporePrint.git
cd sporePrint

# Run validation
cargo run --manifest-path crates/spore-validate/Cargo.toml -- certify

# Compare output with https://sporeprint.primals.eco/certification/manifest.json
```

## The Standard

The verification standard is the same for science, legal, and methodology:

1. **Claim** — every assertion is cited to a source
2. **Source** — every source is publicly accessible or FOIA-obtainable
3. **Hash** — every document is BLAKE3 content-addressed
4. **Repo** — every version is git-signed and timestamped
5. **Surface** — every record exists on multiple independent surfaces

If you find something wrong, [contact us](/about/). Corrections are published and the git history preserves both the original and the correction.
