---
type: Research Guide
title: How the per-book character counts are made
description: The exact rule the book pages use to count how often Butler's translation names each figure, including what is folded together, what is excluded, and where the method is imperfect.
tags:
  - scholarship
  - verification
  - method
  - odyssey
sources:
  - id: butler
    resource: ../external-sources/project-gutenberg-odyssey.md
    title: Project Gutenberg — The Odyssey
---
> [!NOTE]
> Each of the twenty-four [book guides](../story/overview.md) ends with a list of figures and a number. This page states exactly how those numbers are produced, so that a reader who checks them against the source arrives at the same result — and knows where the method is rough.

## The corpus counted

Counts are taken over the [preserved Samuel Butler translation](../external-sources/project-gutenberg-odyssey.md), split at Butler's twenty-four book divisions.[^butler]

Three parts of that file are **not** Butler's translated prose and are excluded:

- Everything before Book 1 — Project Gutenberg's front matter, the contents, and Butler's own prefaces. These name Ulysses nine times outside the poem, and, more awkwardly for a counter, they quote Butcher and Lang's rival translation at length. That passage uses Odysseus, Zeus and Poseidon — forms that occur nowhere in Butler's own twenty-four books, where the same figures are Ulysses, Jove and Neptune. Counting the front matter would therefore introduce names absent from the text being counted, and would also inflate Hyperion, which Butler does write four times inside the poem.

- The ALL-CAPS chapter summary Project Gutenberg places above each book. These are editorial apparatus, not translation, and they name figures freely. Counting them corrupted 65 of the figure-and-book cells — usually by one, six times by two, and once by three — Ulysses in Book 19 — and made the dog Argos appear three times in Book 17 where the translation names him twice. One error survived into the prose as well: the summary of Book 20 said Ctesippus threw an "ox hoof", which is the header's wording ("CTESIPPUS THROWS AN OX'S FOOT"), where Butler's own sentence has him pick "a heifer's foot from the meat-basket".
- Butler's endnotes and the Project Gutenberg licence blocks that follow Book 24.

## What counts as naming a figure

A figure is counted once for each time the translation names them. Because Butler is a Victorian translator working from Greek, "the name" is rarely a single string:

| Rule | Example |
| --- | --- |
| Roman equivalents are the name | Butler writes Ulysses, Minerva, Jove, Neptune, Mercury, Diana, Venus, Mars, Vulcan, Proserpine, Hercules — never Odysseus, Athena, Zeus, Poseidon, Hermes, Artemis, Aphrodite, Ares, Hephaestus, Persephone, Heracles |
| Butler's own spellings are the name | Euryclea, Teiresias, Eupeithes, Alcmena, Clytoneus, Leiodes, Idothea |
| Butler's inconsistencies are folded together | He writes both Halius and Halios for the same son of Alcinous, and both Leiocritus and Leocritus for the same suitor |
| Established alternate names count | Leucothea is Ino after her transformation; Hyperion and "the sun-god" are Helios; "Dawn" and, once, "Aurora" are Eos |
| One standing epithet counts, and only one | Polyphemus is called "the Cyclops" far more often than he is named, and Book 9's sixteen is three namings plus thirteen epithets. This is a deliberate exception, not a general rule: Butler's "the swineherd" (58 times, counting one capitalised vocative), "the stockman" (15, counting two), and "the son of Saturn" for Jove (7) are **not** counted, because a rule that swept in every epithet would measure how often a figure is referred to rather than named |
| Possessives count | "Jove's" is a naming of Jove |
| Names stacked in apposition are one naming | "the Sun-god Hyperion" and "the sun-god son of Hyperion" each name Helios once, not twice. A clause that introduces an alternate name is separate, though: "Ino daughter of Cadmus, also called Leucothea" names her twice, because the second half tells you the other name rather than using it |
| Ties are broken alphabetically | Two figures with the same count appear in order of the name shown in the list |
| A collective name counts for the people, not for one of them | "thousands of sturdy Laestrygonians" counts; "a Laestrygonian named Antiphates" names Antiphates |
| A collective used as an adjective on a place does not count | "the city of the Laestrygonians" counts, because the people own the city; "the Laestrygonian city Telepylos" does not, because there the name is describing the city |

## What does not count

- **Names used as places.** Argos is Odysseus's dog only in Book 17; in seven other books it is the region in the Peloponnese. "the house of Hades" and "down to Hades" name the underworld, not its ruler.
- **Patronymics that identify someone else.** "Eurymachus son of Polybus" names Eurymachus. Butler uses that formula throughout the Ithacan books, and counting it credited a suitor with appearances he never makes — see [Polybus](../characters/polybus.md), where the name belongs to three unrelated men as well as to Eurymachus's father.
- **Ordinary words that share a name's spelling.** "from dawn till dark" is a time of day, not the goddess [Eos](../characters/eos.md).
- **The chapter summaries**, as above.

## Which figures appear in a list

The lists are drawn from the figures that have a guide in this wiki — the [main constellation](../characters/constellation.md) and the [named figures register](../characters/named-figures-register.md) — not from every proper noun in the poem. Butler names many people who have no guide here: minor Phaeacian athletes, most of the sons in the underworld catalogue of women, several suitors named only as they die. A list therefore answers "which figures covered by this wiki does Butler name in this book, and how often", not "who is named in this book".

## Where the method is imperfect

Stated plainly, because a method claim that hides its edges is worse than none:

- **Butler's capitalisation of Dawn is inconsistent.** The rule counts capitalised `Dawn` as the goddess and lowercase `dawn` as a time of day. That is right in most places and wrong in at least two, where the lowercase form is plainly personified: "the child of morning, rosy-fingered dawn, appeared" in Book 9, and "dawn enthroned in gold" in Book 12.
- **Some names carry footnote digits.** The Gutenberg text renders Butler's footnote markers directly against the word, giving `Mentor20` in Book 2, `Menelaus36` in Book 4, and `Eurynome156` and `Eurynome183` in Books 20 and 23. A word-boundary match silently skips all of them, because digits are word characters; the first two are counted here, and Eurynome has no guide in this wiki so she falls outside the lists entirely. Three separate attempts to verify these counts reproduced the same bug, because each used the same regex that caused it.
- **[Hades](../characters/hades.md) is deliberately excluded, and the exclusion is a judgement call rather than a rule.** Butler writes the name exactly thirty times. Twenty-five are plainly the place — "the house of Hades", "the dark abode of Hades", "down to Hades". Three are plainly the god: "prayers to Hades and to Proserpine" in Books 10 and 11, and "the house of the mighty jailor Hades" in Book 11. Two are genuinely undecidable, and they are the same formula twice in Book 10 — "the house of Hades and of dread Proserpine", "the house of Hades and Proserpine" — where the phrase names two gods and a location at once.

  So the doubt is two tokens, not a general impossibility. A count of one for Book 10 and two for Book 11 would be defensible. It is left out anyway, because Hades is the one figure here whose name is overwhelmingly a place, and a small number attached to him would imply a presence in the poem he does not have — the lists would say "Hades (2)" where the honest statement is "Butler names the underworld constantly and its ruler barely at all". That is an editorial preference, and it is recorded here rather than hidden in the data.
- **Frequency is not importance.** Books 9 to 12 are narrated by Odysseus in the first person, so the translation rarely names him: he ranks below Zeus in his own account of the underworld. The counts measure how often a name appears, nothing more.

## Why publish the numbers at all

Because they are checkable. Every other claim in this wiki rests on reading; these rest on counting, and a reader with the preserved text and a `grep` can falsify them in a minute. They have in fact been wrong and corrected four times — 92 cells, then 11, then 2, then 1 — every time because someone counted independently — which is the argument for stating the method rather than the result. The [verification method](./verification-method.md) describes how the wiki's other claims are checked.

[Scholarship overview](./overview.md) · [Textual foundations](./textual-foundations.md) · [Story guide](../story/overview.md)

[^butler]: [Samuel Butler translation](../external-sources/project-gutenberg-odyssey.md)
