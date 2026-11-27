---
title: ~Style Guide~
description: How every page on the Paradise wiki is written and formatted
published: true
date: 2026-11-27T15:17:07.782Z
tags: 
editor: markdown
dateCreated: 2026-11-19T00:22:42.267Z
---

# Style Guide
Every page on the *Paradise* wiki follows these rules, so the wiki reads as one consistent document.

## Page Structure
- Each page has one `#` heading, matching the page title.
- A succinct intro paragraph follows the title, before the first section. It says what the subject is and how it works, linking related mechanics inline as it goes.
- Tables go wherever they fit naturally, in the intro or in a section.
- Sections are only for details this page owns. A section that would only restate another page becomes a phrase with an inline link instead.
- Sections use `##` and subsections use `###`. Nothing deeper than `###`.
- Sections are separated by headings only, never by horizontal rules.

## One Home per Mechanic
Every mechanic is explained, with its numbers, on exactly one page: its home. Other pages mention it in a few words and link to its home, rather than repeating how it works.

- Correct: Swords can land [critical strikes](/weapon_effects#critical-strikes), increasing with skill in [Arms Lore](/arms_lore).
- Incorrect: Swords can land a critical strike, which doubles the hit's damage before armor. Each sword has its own chance, from `10%` for the broadsword to `40%` for the viking sword at `100` Arms Lore. See [Weapon Effects: Critical Strikes](/weapon_effects#critical-strikes).

A number belongs on the page that owns its mechanic, so a change only needs to be made in one place. A table that compares things across pages, such as weapon damage on [Damage Per Second](/dps), is the home for those numbers.

## Headings
Headings use Title Case, with short words (a, an, and, as, at, by, for, in, of, on, or, the, to, with) in lowercase unless they come first.

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

Scripts, macros, and other multi-line code go in a code block: a line of three backticks before the code and another after it, with no language name. A short line before the block says what it is, such as "Example TazUO Legion script:". See [Lockpicking: Macro Training](/lockpicking#macro-training).

## Bold
Bold is only for critical warnings, such as **Pet death is permanent.** It is never used for names, places, or general emphasis.

## Italics
Italics are used for:
- The shard name: *Paradise*
- Text shown in game exactly as worded: the pet *looks happier*

## Capitalization
- Proper names are capitalized: skills (Animal Lore), spells (Magic Reflection), places (Serpent's Hold), NPCs (Grizelda), and named mechanics (Pack Instinct, Loyalty, Valor).
- Ordinary creatures and items are lowercase: dragons, bandages, a treasure map.

## Links
- Page paths are all lowercase, with words separated by underscores: `/animal_taming`, `/treasure_map`. The page title keeps its normal capitalization (Animal Taming); only the path is lowercase.
- Page paths and titles are singular when the page is about one kind of thing (`/pet`, `/house`), and plural when the page is an overview or list (`/skills`, `/dungeons`).
- Links always use a relative path: `/pet`, never `https://paradiseuo.com/pet`.
- Links to a section add an anchor: `/pet#obeying-commands`.
- Anchors must be lowercase, with spaces converted to hyphens and punctuation removed, or they won't work. "Obeying Commands" becomes `#obeying-commands`. `%20` does not work.
- Links go inline, on the words that name the subject: a character defends against the attacker's [hit chance](/combat#hit-chance) with Swordsmanship.
- Each link target is linked only at its first mention on a page. A page and each of its sections are separate targets, so `/combat#damage` and `/combat#hit-chance` can each be linked once on the same page.
- Links to pages that don't exist yet are kept. They mark planned pages and start working once the page is written.
- Link text follows normal sentence capitalization: capitals only for proper names, such as skills, spells, and places. Ordinary words stay lowercase.
  - Examples: tamers turn animals into [pets](/pet), healed with [Veterinary](/veterinary), listed in the [patch notes](/patch_notes)

### See Links
A "See" link is a last resort, for when no word in the sentence can carry the link. It uses the title of what it links to: the page's title for a whole page, such as See [Stable](/stable), or the section's heading for a section. If the heading is too vague to stand on its own, the page title and a colon go before it, such as See [Combat: Damage](/combat#damage).

- Correct: Each weapon's speed and damage are listed on [Damage Per Second](/dps).
- Incorrect: Each weapon has its own speed and damage. See [Damage Per Second](/dps).

## Notes and Warnings
The wiki doesn't use note boxes, callouts, or block quotes. Important information goes in the text, with bold for critical warnings.

A detail that hasn't been checked against the server's code ends with (unconfirmed), in plain text, before the sentence's final punctuation. The marker is removed once the detail is checked. Example: A thrown potion adds `Alchemy / 10` damage (unconfirmed).

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
- Minus signs use a plain hyphen, not a longer dash: -50%, `(Healing - 30) / 50`.

## Formulas
Formulas use full skill and stat names, never abbreviations.
- Correct: `(Veterinary + 10)%`
- Incorrect: `(vet + 10)%`

## Writing
- American spelling: armor, color, gray, center, -ize endings (capitalize, organize).
- In-game names keep their in-game spelling, even when it's British: a grey wolf.
- Paired female and male words put the female form first: Lady/Lord.
- The Oxford comma is always used: Animal Taming, Animal Lore, and Veterinary.
- Other commas are used only where they help the reader. A comma that can be removed without changing the meaning or making the sentence harder to read is removed. A sentence that needs three or more commas is usually better split in two.
  - Correct: Fists do `1` to `8` damage before bonuses and swing quickly.
  - Incorrect: Fists do `1` to `8` damage before bonuses, and swing quickly.
- Third person, present tense: players, a tamer. Not "you".
- Instructions are third person too, never commands to the reader: "Double-clicking a treasure map decodes it," not "Double-click a treasure map." Patch notes are the one exception, and are written as commands, such as "Add the Lich King".
- No emoji.
- No superscript. Notes go in plain text, usually in parentheses or as their own sentence.

## Skill Pages
Every skill page ends with two sections, in this order, even if they're still empty:
1. `## Manual Training`
1. `## Macro Training`

These two sections can be written with some levity, since players read them while grinding. Every other rule still applies.

## Paradise Changes
Reworks, meaning novel systems or large reworks of existing ones such as Valor, each get their own section on the [Features](/features) page. Other novel changes are listed there under Other Changes. Small tweaks, quality-of-life changes, and changes made to match T2A go only in the [patch notes](/patch_notes), even when they differ from other versions of Ultima Online.

Other pages describe each change as part of how the game works, without flagging it as a change.