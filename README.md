---
type: Document
title: The Odyssey — OpenKnowledge example
description: A public example of a deeply researched, interconnected OKF knowledge base.
tags:
  - readme
  - openknowledge
  - okf
  - odyssey
  - example
---
[Read this wiki using OpenKnowledge!](https://openknowledge.ai/d/AWh0dHBzOi8vZ2l0aHViLmNvbS9pbmtlZXAvb2R5c3NleS1va2Ytd2lraS9ibG9iL21haW4vUkVBRE1FLm1k)

---

This repository is a public example of using **OpenKnowledge** and the **Open Knowledge Format (OKF)** to build a rich, durable knowledge base around a substantial subject.

The subject is Homer’s *Odyssey*. The wiki connects all twenty-four books with character guides, themes, historical and poetic context, translations, adaptations, scholarship, and locally preserved source records.

## Start here

Open [The Odyssey](home.md) for the reader-facing wiki, or inspect the root [OKF index](index.md) to see the portable bundle structure.

## What this example demonstrates

- One Markdown document per useful concept, with typed YAML frontmatter
- Standard Markdown links forming a navigable knowledge graph
- Section indexes and reusable folder templates
- Citations that resolve to local source records rather than to live URLs, so the evidence travels with the bundle — with one disclosed exception, the [reception pages](reception/overview.md), whose subjects are films, novels and comics the repository cannot preserve
- Clear separation between primary texts, metadata-only web sources, and editorial synthesis
- Explicit generation, verification, provenance, and rights metadata
- A chronological [work log](log.md) for durable maintenance history
- Machine-checkable OKF conformance, Markdown quality, and internal-link integrity

The collection is designed to remain readable as ordinary Markdown while gaining richer navigation, templates, provenance, validation, and collaborative editing when opened in OpenKnowledge.

## How this wiki was written

The editorial content here was drafted by an AI agent working through OpenKnowledge, then verified against the preserved sources in this repository. Most pages record that origin in their own frontmatter under a `generated:` key, so you can see per document what produced it and when.

That provenance is the point of the example rather than a disclaimer on it: agent-authored knowledge is only trustworthy when every claim resolves to a source a reader can open, and the [verification method](scholarship/verification-method.md) documents how claims here were checked. Treat the pages as a well-sourced reading companion, not as peer-reviewed scholarship — where a page matters to your own work, follow its citation to the underlying text.

## Opening this repo in an agent client

This repository carries a committed [`.mcp.json`](.mcp.json) (and an equivalent `.codex/config.toml`), so Claude Code, Codex, and similar clients will offer to start the OpenKnowledge MCP server when you open the folder. Approving that prompt runs a small shell script that prefers an installed OpenKnowledge desktop app and otherwise falls back to `npx`. The npm fallback is pinned to a version range rather than `@latest`, so what a cloner runs is the range this repository was checked against. Nothing starts without your approval, and the wiki reads perfectly well as plain Markdown if you decline.

## Repository map

| Area | Contents |
| --- | --- |
| [Story](story/overview.md) | Narrative architecture and guides to all twenty-four books |
| [Characters](characters/constellation.md) | Major figures, minor figures, gods, monsters, and communities |
| [Themes](themes/overview.md) | Return, hospitality, cunning, recognition, storytelling, justice, and more |
| [World](world/overview.md) | Composition, poetics, geography, institutions, religion, labor, and objects |
| [Reception](reception/overview.md) | Translations and afterlives across literature, film, television, and art |
| [Scholarship](scholarship/overview.md) | Textual foundations, reading pathways, and verification methods |
| [Sources](external-sources/index.md) | Local primary texts and rights-aware provenance records |

## Reuse

Original wiki-authored content is available under the terms in [License](LICENSE.md) — CC BY 4.0, with the full legal code in [`LICENSE`](LICENSE). Preserved texts, catalog data, names, and linked publications retain their own terms; see [Third-party notices](THIRD-PARTY-NOTICES.md).

## Contributing

Corrections and additions are welcome, and are held to the sourcing standard described in [Contributing](CONTRIBUTING.md). Participation is governed by the [code of conduct](CODE_OF_CONDUCT.md).
