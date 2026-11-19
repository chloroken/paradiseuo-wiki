---
title: Reputation
description: 
published: true
date: 2026-11-19T05:34:04.982Z
tags: 
editor: markdown
dateCreated: 2026-11-14T06:31:40.281Z
---

# Reputation
A character's reputation 𐠒 is made of two values: Fame and Karma, and together they determine a character's [title](#titles) and benefits.

## Fame
Fame measures how respected a character is by other citizens, and gives different bonuses depending on how famous a character is. At high Fame, jewelers pay more for gems. At low Fame, the chance of skill gain is higher. Fame gains slow down as Fame rises.

| Fame | Title | Gem Sale Bonus (%) | Skill Gain Bonus (%) |
|:-|:-:|:-:|:-:|
| 0 – 1,249 | — | 0 | 10 |
| 1,250 – 2,499 | Notable | 2.5 | 7.5 |
| 2,500 – 4,999 | Prominent | 5 | 5 |
| 5,000 – 9,999 | Renowned | 7.5 | 2.5 |
| 10,000+ | Lady/Lord | 10 | 0 |

### Gaining and Losing Fame
Fame is gained by:
- Killing monsters. Stronger monsters give more Fame.
- Donating gold to NPCs, at `1` Fame per `100` gold.

Fame is lost by:
- Being resurrected, at `10%` each time.

## Karma
Karma measures good and evil. Karma changes slow down the further a character strays from neutral, except for changes from templars and thugs. Most monsters are evil, so hunting monsters naturally raises Karma. Keeping Karma negative takes thought and planning.

### Gaining and Losing Karma
Karma is gained by:
- Killing evil monsters.
- Killing thugs.

Karma is lost by:
- Killing good creatures.
- Successfully [begging](/begging).
- Killing templars.

### Templars and Thugs
Templars are good NPCs and thugs are evil ones, found outside the teleporters to their karma towns.

- They attack players whose Karma is opposite to theirs.
- They give no Fame and drop poor loot.
- Each kill changes Karma by `25` to `75`.
- Beyond `5,000` or `-5,000` Karma, the change is halved.
- Every player who damaged the NPC receives the full Karma change.

### Karma Towns
The people of these two towns only deal with characters of the right karmic persuasion.

| Town | Required Karma | Teleporter |
|:-|:-:|:-:|
| Serpent's Hold | 5,000+ | Guard outpost north of Trinsic |
| Buccaneer's Den | -5,000 or below | Crossroads west of Vesper |

- Vendors, bankers, animal trainers, healers, trainers, and hirelings in these towns refuse to deal with characters who don't meet the requirement.
- Neither town has a moongate. Travel there by boat, by magic, or by teleporter.

### Karma Lock
- If Karma drops from positive to below `0`, it becomes locked.
- Locked Karma can't be increased by any means, but it can still decrease.
- To unlock it, stand beside the ankh at any shrine and speak that shrine's mantra.

| Shrine | Mantra |
|:-|:-:|
| Honesty | `Ahm` |
| Compassion | `Mu` |
| Valor | `Ra` |
| Justice | `Beh` |
| Sacrifice | `Cah` |
| Honor | `Summ` |
| Spirituality | `Om` |
| Humility | `Lum` |

## Limits
| Value | Minimum | Maximum |
|:-|:-:|:-:|
| Fame | 0 | 32,000 |
| Karma | -32,000 | 32,000 |

## Titles
Fame and Karma combine to create a character's title.

| Karma | Below 1,250 Fame | Below 2,500 Fame | Below 5,000 Fame | Below 10,000 Fame | 10,000+ Fame |
|:-|:-:|:-:|:-:|:-:|:-:|
| 10,000+ | Trustworthy | Estimable | Great | Glorious | Glorious Lady/Lord |
| 5,000+ | Honest | Commendable | Famed | Illustrious | Illustrious Lady/Lord |
| 2,500+ | Good | Honorable | Admirable | Noble | Noble Lady/Lord |
| 1,250+ | Kind | Respectable | Proper | Eminent | Eminent Lady/Lord |
| 625+ | Fair | Upstanding | Reputable | Distinguished | Distinguished Lady/Lord |
| -624 – 624 | — | Notable | Prominent | Renowned | Lady/Lord |
| -625 or below | Rude | Disreputable | Notorious | Infamous | Dishonored Lady/Lord |
| -1,250 or below | Unsavory | Dishonorable | Ignoble | Sinister | Sinister Lady/Lord |
| -2,500 or below | Scoundrel | Malicious | Vile | Villainous | Dark Lady/Lord |
| -5,000 or below | Despicable | Dastardly | Wicked | Evil | Evil Lady/Lord |
| -10,000 or below | Outcast | Wretched | Nefarious | Dread | Dread Lady/Lord |
