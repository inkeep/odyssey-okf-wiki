---
type: Method
title: Verification method
description: A reproducible protocol for checking structure, provenance, textual claims, interpretations, and review status.
tags:
  - verification
  - method
  - odyssey
sources:
  - id: greek
    resource: ../external-sources/perseus-greek-odyssey.md
    title: Perseus Digital Library Greek Odyssey
  - id: butler
    resource: ../external-sources/project-gutenberg-odyssey.md
    title: Complete Samuel Butler translation
generated:
  by: openai/codex
  at: 2026-08-18T14:50:00-07:00
---
## What “verified” means here

Verification is claim-specific. A clean automated audit proves that the knowledge base is structurally coherent; it does not prove that every interpretation is correct.

## Reproducible checks

1. Run the OpenKnowledge project audit and require zero lint findings and zero dead internal links.
2. Confirm every external source used by an article has a local wrapper.
3. For preserved assets, compare recorded byte counts and SHA-256 checksums.
4. Check plot, speaker, sequence, and named-figure claims against the complete primary text.[^butler]
5. Where English wording matters, consult the preserved Ancient Greek edition rather than treating one translation as identical with Homeric Greek.[^greek]
6. Label interpretive conclusions as arguments and preserve reasonable alternatives.
7. Reserve human verification for an identified reviewer; never infer it from automated checks.

## Review record

| Area | Current status |
| --- | --- |
| Markdown and internal links | Fully machine-audited |
| Source wrappers and preserved assets | Checked for presence and recorded integrity metadata |
| Plot sequence and character identification | Grounded in the complete Butler text |
| Greek wording and textual variants | Source available; not exhaustively collated |
| Interpretive essays | Source-linked arguments, not peer review |
| Scholarly bibliography | Catalog-verified; argument summaries remain editorial guidance |
| Independent classicist review | Not yet performed |

## How to review a page

Follow its footnote into the local source, locate the relevant book or passage, then distinguish what the text states from what the article infers. Record any human review with the reviewer's identity, date, and scope; never apply a blanket verification flag for a partial check.

[Scholarship overview](./overview.md) · [Textual foundations](./textual-foundations.md)

[^butler]: [Complete Samuel Butler text](../external-sources/project-gutenberg-odyssey.md)
[^greek]: [Perseus Greek Odyssey](../external-sources/perseus-greek-odyssey.md)
