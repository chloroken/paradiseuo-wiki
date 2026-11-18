---
title: ~Wiki Style Guide
description: 
published: true
date: 2026-11-18T23:06:27.740Z
tags: 
editor: markdown
dateCreated: 2026-11-18T22:08:53.727Z
---

---
title: ~Wiki Style Guide
description: 
published: true
date: 2026-11-18T22:55:19.435Z
tags: 
editor: markdown
dateCreated: 2026-11-18T22:08:53.727Z
---

# Style Guide
Every page on the *Paradise* wiki follows these rules, so the wiki reads as one consistent document.

## Page Structure
- Each page has one `#` heading, matching the page title.
- A short intro paragraph follows the title, before the first section.
- Sections use `##` and subsections use `###`. Nothing deeper than `###`.
- Sections are separated by headings only, never by horizontal rules.

## Headings
Headings use Title Case, with short words (a, an, and, as, at, by, for, in, of, on, or, the, to) in lowercase unless they come first.

- Correct: Training on Pets
- Incorrect: Training On Pets

## Backticks
Backticks are used for exactly four things:

1. **Game values:** any number set by the shard's rules, which could change if the code changed. This includes percentages, durations, skill amounts, and counts.
   - Correct: a `10` second cooldown, `3` spawns per day, a `50%` chance
   - Incorrect: 24 hours in a day, two keys
1. **Formulas:** `(4 * Animal Taming + Animal Lore) / 5`
1. **Exact input:** anything typed or entered exactly as written, including speech commands, keys, and values entered into a client or macro.
   - Examples: `all follow me`, `claim <name>`, `Alt + Click`, `*pet*`
1. **Filenames and on-screen labels:** files, buttons, menus, and fields exactly as they appear on screen.
   - Examples: `TazUOLauncher.exe`, `Plot Course`, `Profile Name`

Commands are never wrapped in quotation marks inside backticks.

Backticks are never used inside tables, with one exception: exact input, filenames, and on-screen labels keep their backticks, such as in a command table.

## Bold
Bold is only for critical warnings, such as **Pet death is permanent.** It is never used for names, places, or general emphasis.

## Italics
Italics are used for:
- The shard name: *Paradise*
- Text shown in game exactly as worded: the pet *looks happier*

## Capitalization
- Proper names are capitalized: skills (Animal Lore), spells (Magic Reflection), places (Serpent's Hold), NPCs (Grizelda), and named mechanics (Pack Instinct, Loyalty).
- Ordinary creatures and items are lowercase: dragons, bandages, a treasure map.

## Links
- Page paths are all lowercase, with words separated by underscores: `/animal_taming`, `/treasure_map`. The page title keeps its normal capitalization (Animal Taming); only the path is lowercase.
- Page paths and titles are singular when the page is about one kind of thing (`/pet`, `/house`), and plural when the page is an overview or list (`/skills`, `/dungeons`).
- Links always use a relative path: `/pet`, never `https://paradiseuo.com/pet`.
- Links to a section add an anchor: `/pet#obeying-commands`.
- Anchors must be lowercase, with spaces converted to hyphens and punctuation removed, or they won't work. "Obeying Commands" becomes `#obeying-commands`. `%20` does not work.
- Only the first mention of a page is linked on any given page.
- Cross-references are written as: See [Stable](/stable).

## Notes and Warnings
The wiki doesn't use note boxes, callouts, or block quotes. Important information goes in the text, with bold for critical warnings.

## Lists
- Unordered lists use `-`.
- Numbered lists are only used when order or rank matters, and every item is written as `1.` so Wiki.js numbers them automatically.
- List items that are full sentences end with a period. Fragments have no period.

## Tables
- The first column is left-aligned, and all other columns are centered: `|:-|:-:|:-:|`
- No backticks inside tables, except for exact input.
- When every row shares a unit, it goes in the header: Delay (s), Range (tiles).
- Ranges use an en dash with spaces: 60 – 74.9
- Thresholds are written as: Below 40, 40 – 99, 100+

## Numbers
- Decimals only where they matter: 59.1, 100, 0 (not 100.0 or 0.00).
- Thousands use commas: 32,000
- Ranges in prose use "to": lasts 10 to 120 seconds.

## Formulas
Formulas use full skill and stat names, never abbreviations.
- Correct: `(Veterinary + 10)%`
- Incorrect: `(vet + 10)%`

## Writing
- American spelling: armor, color, gray, center, -ize endings (capitalize, organize).
- The Oxford comma is always used: Animal Taming, Animal Lore, and Veterinary.
- Third person, present tense: players, a tamer. Not "you".
- No emoji.
- No superscript. Notes go in plain text, usually in parentheses or as their own sentence.

## Skill Pages
Every skill page ends with two sections, in this order, even if they're still empty:
1. `## Manual Training`
1. `## Macro Training`

## Paradise Changes
Features that differ from standard Ultima Online are marked with 𐠒 after their name, on any page where they appear. Every marked feature is also listed on the [Novelties](/novelties) page.
