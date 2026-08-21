---
type: Attribution Notice
title: Third-party notices
description: Attribution, provenance, and reuse boundaries for external material in the wiki.
tags:
  - attribution
  - provenance
  - license
  - governance
---
This repository combines original editorial material with preserved primary texts, open scholarly data, and metadata-only records of copyrighted web pages. The repository-level [license](LICENSE.md) covers only original wiki-authored content.

## Perseus Digital Library Greek text

- Material: [machine-readable Ancient Greek *Odyssey*](external-sources/perseus-greek-odyssey.md)
- Creator and publisher: Homer; edited by Augustus Taber Murray; prepared under the supervision of the Perseus Project, Tufts University, with Gregory Crane as principal; published by the Trustees of Tufts University
- Source edition: Loeb Classical Library (Heinemann / Putnam, 1919)
- Upstream collection: `PerseusDL/canonical-greekLit`
- Terms: Creative Commons Attribution-ShareAlike 4.0 International (`https://creativecommons.org/licenses/by-sa/4.0/`) unless a component says otherwise
- Changes here: none to the preserved XML bytes; the wiki adds a separate wrapper and checksum

Reuse must preserve attribution, identify changes, link to the upstream material and license, and apply ShareAlike when the license requires it. Note that the TEI header of this particular file carries no rights element; the licence statement comes from the upstream repository, not from the file. Perseus additionally asks that modifications be offered back to the project, and describes its materials as provided for the personal use of students, scholars, and the public — terms that sit outside the Creative Commons licence and that reusers should evaluate for themselves.

ShareAlike does not reach the rest of this wiki. CC BY-SA 4.0 imposes ShareAlike on *Adapted Material*; the XML is preserved unmodified in its own file with its own record, which makes this a collection rather than an adaptation. No wiki page reproduces the Greek text.

## Samuel Butler translation

- Material: [complete Samuel Butler translation](external-sources/project-gutenberg-odyssey.md)
- Source: Project Gutenberg ebook 1727
- Copyright status: identified by Project Gutenberg as unrestricted by United States copyright law
- Changes here: none to the preserved text bytes

The preserved ebook contains the Project Gutenberg license. Redistribution while retaining the Project Gutenberg name or association must follow that license and its trademark conditions. Copyright status can differ outside the United States.

## Open Library catalog response

- Material: [catalog query response](external-sources/open-library-odyssey-bibliography.md)
- Source: Open Library, an Internet Archive project
- Changes here: none to the preserved JSON bytes

Open Library states that the Internet Archive asserts no new copyright or proprietary rights over its database, while warning that existing rights may apply to contributions or in some jurisdictions. Reusers should preserve provenance and assess their jurisdiction and use.

## Bundled agent skill

- Material: `.claude/skills/okf-knowledge-base/` and its identical `.codex/` copy
- Creator: Inkeep
- Upstream: `https://github.com/inkeep/open-knowledge-skills`
- Changes here: none; the files are vendored as imported, and `.ok/skills-lock.json` records the content hash

The skill describes the Open Knowledge Format contract this bundle demonstrates and is committed so that a cloner gets it without a separate install step. It carries no license header upstream; consult the upstream repository for its terms.

## Copyrighted websites

The records below preserve only limited factual metadata, original wiki summaries, and retrieval URLs. They do not license or reproduce the linked pages:

- [Encyclopaedia Britannica](external-sources/britannica-odyssey.md)
- [Center for Hellenic Studies](external-sources/chs-homer-multitext.md)
- [Emily Wilson](external-sources/emily-wilson-odyssey.md)
- [Hackett Publishing](external-sources/hackett-lombardo-odyssey.md)
- [History](external-sources/history-adaptations.md)
- [Metropolitan Museum of Art](external-sources/met-odyssey-1806.md)
- [Penguin Random House](external-sources/penguin-fagles-odyssey.md)

Names and trademarks belong to their respective owners. Linking or attribution does not imply endorsement.

## No legal advice

This notice documents provenance and intended reuse boundaries; it is not legal advice. Reusers remain responsible for complying with applicable law and source-specific terms.
