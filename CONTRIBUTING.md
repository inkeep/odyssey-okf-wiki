---
type: Contribution Guide
title: Contributing
description: How to propose corrections and additions to this wiki, and the sourcing standard every change must meet.
tags:
  - contributing
  - governance
  - okf
---
Corrections and additions are welcome. This wiki is also a worked example of the [Open Knowledge Format](README.md), so contributions are held to the same sourcing and structural standard as the existing pages.

## What is most useful

- **Corrections with a citation.** A factual fix that names the source it rests on is the single most valuable contribution here.
- **Deeper coverage of an existing page.** Minor figures, themes, and reception strands all have room to grow.
- **New source records.** A preserved public-domain text or an open catalog response, captured under [external sources](external-sources/index.md) with rights metadata.

Please open an issue before starting a large restructuring, so the effort is not wasted on a direction the maintainers would not merge.

## The sourcing standard

Every factual claim must cite a source that a reader can open, and that source must live inside this repository:

- Cite with an ordinary Markdown link to a local record: `[Samuel Butler translation](external-sources/project-gutenberg-odyssey.md)`.
- A bare link to an external website is **not** a citation. If a web page is the evidence, add a source record for it under `external-sources/` first, then cite that record.
- Respect the rights boundary described in [Third-party notices](THIRD-PARTY-NOTICES.md). Preserve full text only where redistribution is permitted; otherwise capture metadata and write an original summary.
- If you cannot source a claim, leave it out. Unsourced assertion is the one thing this example is trying to demonstrate the absence of.

One part of the wiki cannot meet that bar and says so. The [reception pages](reception/overview.md) describe films, novels and comics that cannot be preserved here for copyright reasons, so their readings come from the works themselves rather than from a record in this repository. Where that is true, the page states it at the point of use. Treat it as a disclosed exception, not a licence: everywhere else, cite a local record.

The [verification method](scholarship/verification-method.md) describes how existing claims were checked and what the confidence levels mean.

## Structural conventions

- One document per concept, as Markdown with YAML frontmatter. `title` and `description` are required; `tags` are expected.
- Use the folder's template when one exists. Each content folder advertises its templates through OpenKnowledge.
- Link with relative Markdown links, resolved from the page you are editing: from a page inside `themes/`, Odysseus is `[Odysseus](../characters/odysseus.md)`; from the repository root he is `[Odysseus](characters/odysseus.md)`. Every link must resolve.
- `index.md` files are generated. Do not hand-edit them.
- Add a dated entry to the [work log](log.md) describing what you changed and why.

## Checking your work

With OpenKnowledge installed, from the repository root:

```sh
ok audit
```

This reports Markdown-lint violations and broken internal links together. A contribution should leave the audit clean. Opening the repository in an agent client that supports MCP gives the same checks interactively — see [Opening this repo in an agent client](README.md).

## Licensing of contributions

By proposing a change you agree that your original wiki-authored content is contributed under the same terms as the rest of the wiki: **CC BY 4.0**, as set out in the [license](LICENSE.md). Do not contribute third-party text that you are not entitled to license on those terms.

## Conduct

Participation is governed by the [code of conduct](CODE_OF_CONDUCT.md).
