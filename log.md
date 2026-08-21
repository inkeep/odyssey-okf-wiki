---
title: Work Log
description: Chronological record of substantive changes to this knowledge base.
type: Work Log
---
## 2026-08-20: Converged an independent audit loop

- Ran eleven rounds of cold audit against this wiki, each by a reviewer with no knowledge of the previous rounds' conclusions, fixing what each found and re-auditing. Ten rounds produced changes; the last three found nothing blocking. Blocking findings fell from 101 wrong count entries in the first round to none.
- Corrected the per-book counts four times — 92 cells, then 11, then 2, then 1 — and documented the whole method, its exclusions and its known imperfections on [how the per-book counts are made](scholarship/counting-method.md).
- Reconciled thirteen character guides whose "Where to read" lists claimed fewer books than the counts credit them with, and made the folder templates describe the pages that actually exist rather than shapes no page used.
- Removed seventeen frontmatter source declarations that no page cited, so the provenance metadata no longer overstates the evidence base.
- Disclosed, in the README and at the point of use, that the reception pages describe works this repository cannot preserve, and that their readings are the wiki's own rather than claims carried by a local record.
- A note on this log: earlier entries have been corrected in place where they turned out to be wrong — a figure that no longer held, a claim about what was removed. The description above no longer calls the log append-only, because it is not.

## 2026-08-20: Acted on an independent pre-publication audit

- Recomputed every per-book character count directly from the preserved Butler translation, after an independent audit found the published figures wrong in three separate ways: four names doubled in every book they appeared in, collectives over-counted, and Project Gutenberg's chapter summaries counted as though they were Butler's prose. A second audit round then found the recount itself still wrong in fourteen places — a header remnant leaking past the stripper, the goddess Eos counted wherever the common noun "dawn" appeared, patronymics counted as though they named the man himself, and an unresolved Halius/Halios spelling. Both classes were fixed, and each book page now links [how the per-book counts are made](scholarship/counting-method.md), which states the rule in full.
- Stopped counting `Hades` as a character where Butler uses it as a place. Book 11's list had been headed by "Hades (20)" against an actual 2, ranking a location above the narrator; the same place-versus-character rule already applied to Argos. A later round removed Hades from the counts altogether — twenty-five of his thirty appearances are the underworld, not its ruler — and the reasoning now lives on [how the per-book counts are made](scholarship/counting-method.md).
- Dropped [Actoris](characters/actoris.md) from the Book 23 count list, since Butler never uses the name — his translation says only "the daughter of Actor". Her guide page remains, and now records that the name comes from the Greek rather than from Butler. Restored [Leiocritus](characters/leocritus.md) to Book 2, where a spelling variant had hidden him.
- Stated the counting basis on all twenty-four pages. A later round showed the basis was still not sufficient to reproduce the numbers — it named the exclusions but not what the counts fold together — so the full rule now lives on one page, [how the per-book counts are made](scholarship/counting-method.md), which the book pages link.
- Corrected [Polybus](characters/polybus.md), which had credited him with a necklace Butler gives to [Pisander](characters/pisander.md) and merged three unrelated men of that name plus a patronymic.
- Replaced fifteen callout types that GitHub does not render, including the opening and closing callouts of the [home page](home.md).
- Added the Project Gutenberg Section 1.E.1 notice to the [source record](external-sources/project-gutenberg-odyssey.md), completed the Perseus attribution with its editor and source edition, hyperlinked the ShareAlike licence, removed a pointer to rights information the XML header does not contain, and recorded why ShareAlike does not reach the rest of the wiki.
- Completed the Contributor Covenant attribution with a licence URI, and backfilled rights metadata on the Britannica and Metropolitan Museum records.
- Pinned the OpenKnowledge npm and schema references to a version range instead of `@latest`, and added a repository-level ignore for the editor settings file that pre-approves the MCP server.

## 2026-08-20: Prepared the repository for public release

- Merged the book-page repair onto `main`, which had still been serving the twenty-four pages with 42 broken character links and the placeholder movement table.
- Added the complete CC BY 4.0 legal code as a plain-text `LICENSE` file and recorded the `CC-BY-4.0` SPDX identifier on the [license](LICENSE.md) page, so automated license detection resolves the grant.
- Disclosed in the [README](README.md) that the editorial content was drafted by an AI agent and verified against the preserved sources, and pointed readers at the [verification method](scholarship/verification-method.md).
- Documented that the committed MCP configuration will offer to start an OpenKnowledge server when the repository is opened in an agent client.
- Replaced the OpenKnowledge-only tab components on the home page and the story map with ordinary Markdown headings, so both render for readers browsing the repository on the web.
- Added a [contributing guide](CONTRIBUTING.md) stating the local-citation sourcing standard and a [code of conduct](CODE_OF_CONDUCT.md).
- Generalized an over-specific note in an earlier log entry and recorded why one agent skill is committed while the other is not.

## 2026-08-20: Repaired the twenty-four book pages

- Rebuilt every book's character list from a per-book occurrence count taken over the preserved Butler translation, with name variants resolved; 42 broken links that had been generated by template-filling a prose sentence as a character name became 508 links that all resolve. Four later audit rounds corrected the counts — 92 cells, then 11, then 2, then 1 — and reduced the entries to 489.
- Listed each book's figures in descending order of how often the translation names them, and stated that basis on the page so a reader can check it against the source.
- Excluded the `Argos` entry from the seven books where the counted name is the Greek region rather than Odysseus's hunting dog, verified line by line against the Butler text; the dog is retained only in Book 17, where he appears.
- Replaced the identical placeholder "Dramatic movement" table on all twenty-four pages with three pressure / response / result beats per book, drawn from that book's own action.
- Replaced the Obsidian-only embed on the Project Gutenberg source record with an ordinary Markdown link to the preserved text, matching the Perseus record so both render for readers outside Obsidian.
- Re-ran the project audit: no broken internal links across 197 documents.

## 2026-08-19: Added a public repository introduction

- Added a concise root README explaining the project’s purpose, structure, OKF features, starting points, and reuse boundaries.
- Kept the OKF bundle at repository root so it opens directly without an unnecessary wrapper directory.

## 2026-08-19: Closed public-release licensing gaps

- Licensed original wiki-authored content under CC BY 4.0 while excluding third-party material.
- Added a consolidated third-party notice for Perseus, Project Gutenberg, Open Library, and copyrighted websites.
- Replaced five copyrighted website extracts with metadata-only source records and original summaries.
- Added source-specific rights, license, modification, and jurisdiction metadata to preserved assets.
- Made the external-source folder and reusable capture template rights-aware.
- Exposed licensing and attribution from the wiki home page.

## 2026-08-19: Hardened the repository for public release

- Replaced five raw website captures with focused text-extracted source records.
- Reduced those captures to factual metadata, discarding the embedded page furniture that raw web captures carry.
- Normalized Git authorship metadata across the repository history.
- Re-ran personal-data, credential-pattern, Markdown, and internal-link audits.

## 2026-08-18: Catalog-verified the scholarly bibliography

- Checked every retained bibliographic recommendation against a preserved Open Library catalog response.
- Normalized recommendations into specific works with authors, first-publication years, publishers, and selected ISBNs where supported.
- Removed vague Stanford and Vernant / Vidal-Naquet recommendations that did not identify a unique edition or title.
- Recorded process-level verification provenance and promoted the bibliography from draft to stable.
- Preserved the full catalog response with byte count and SHA-256 checksum.

## 2026-08-18: Added scholarly and verification apparatus

- Preserved a complete machine-readable Ancient Greek *Odyssey* from PerseusDL with byte count and SHA-256 checksum.
- Added an explicit confidence ladder, reproducible verification method, textual-foundations guide, and purpose-driven scholarly reading pathways.
- Deepened film, literary, and visual-art reception essays and corrected their source attribution.
- Added a close-reading method for minor figures and exposed scholarship from the home page.
- Labeled metadata-only source records truthfully instead of implying raw preservation.

## 2026-08-18: Verified and deepened the wiki

- Preserved the complete Samuel Butler translation and four research pages as local, checksum-recorded source assets.
- Rebuilt the translation guide with edition-specific provenance and grounded oral-composition coverage in the Homer Multitext project.
- Added fifty-four secondary character guides plus a named-figures register, bringing the character collection to 114 figure and collective pages, alongside its navigation and method pages.
- Corrected generated timestamps and primary-source mappings, repaired navigation, and completed a full lint and link audit.

## 2026-08-18: Built the Odyssey wiki

- Created a visual home page and hubs for story, characters, themes, context, and reception.
- Added all twenty-four book guides, sixty character and collective pages, ten theme essays, eight context pages, and seven translation/adaptation studies.
- Ingested five local source records and connected factual claims through OKF provenance and footnotes.
- Added reusable folder templates, corrected the Agamemnon page path, and removed obsolete starter folders.
- Saved checkpoint `9486c989d6b057f752af201c5a4022882f40aa72` before destructive cleanup.
