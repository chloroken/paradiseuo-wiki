---
title: Reputation
description: 
published: true
date: 2026-11-18T22:09:51.657Z
tags: 
editor: markdown
dateCreated: 2026-11-14T06:31:40.281Z
---

# Reputation
A character's reputation is made of two values: **fame** and **karma**. Each value offers its own unique benefits, and together they determine a character's [title](/Reputation#titles).

## Fame
Fame measures how respected a character is by other citizens. Fame offers different bonuses depending on how famous one is: at high fame, `jewelers` pay more for `gems`; at low fame, `skill gain` chance is increased. Fame gains slow down as fame increases.

| Fame | Title | Gem Sale Bonus | Skill Gain Bonus |
|:-:|:-:|:-:|:-:|
| 0 – 1,249 | — | 0% | 10% |
| 1,250 – 2,499 | **Notable** | 2.5% | 7.5% |
| 2,500 – 4,999 | **Prominent** | 5% | 5% |
| 5,000 – 9,999 | **Renowned** | 7.5% | 2.5% |
| 10,000+ | **Lady** / **Lord** | 10% | 0% |

**Fame is gained by:**
- Killing monsters; stronger monsters give more fame.
- Donating `gold` to NPCs, at `1` fame per `100` gold.

**Fame is lost by:**
- Being resurrected (`10%` each time).

## Karma
Karma measures `good` and `evil`. Karma changes slow the further away from `neutral` one strays, with the exception of changes from **Templars** and **Thugs**. Because most monsters are `evil`, hunting monsters will naturally increase karma. Thus, to maintain negative karma requires thought and planning.

**Karma is gained by:**
- Killing evil monsters.
- Killing `Thugs`.

**Karma is lost by:**
- Killing good creatures.
- Successfully [begging](/Begging).
- Killing `Templars`.

**Templars and Thugs:**
- Attack players with karma opposite theirs.
- Don't give fame and drop poor loot.
- Located outside of their respective **karma town** teleporters.
- Each kill changes karma by `25` to `75`.
- Beyond `5,000` or `-5,000`, the karma change is halved.
- Every player who damaged the NPC receives the full karma change.

**Karma Towns:**
- The people of these two towns only deal with characters of the right karmic persuasion.

| Town | Required Karma | Teleporter |
|:-:|:-:|:-:|
| **Serpent's Hold** | `>= 5,000` | Guard outpost north of Trinsic | 
| **Buccaneer's Den** | `<= -5,000` | Crossroads west of Vesper |

- `Vendors`, `bankers`, `stablemasters`, `healers`, `trainers`, and `hirelings` in these towns refuse to deal with characters who don't meet the requirement.
- Neither town has a `moongate`. Travel there by `boat`, by magic, or by `teleporter`.

**Karma Lock:**
- If karma drops from positive to below `0`, it will become **locked**.
- Locked karma cannot be increased by any means, but it can still decrease.
- To unlock normal gains, one must interact with an `ankh` at any `shrine`.
- Stand beside the ankh and speak that shrine's specific mantra.

| Shrine | Mantra |
|:-:|:-:|
| Honesty | `Ahm` |
| Compassion | `Mu` |
| Valor | `Ra` |
| Justice | `Beh` |
| Sacrifice | `Cah` |
| Honor | `Summ` |
| Spirituality | `Om` |
| Humility | `Lum` |

## Limits
| | Minimum | Maximum |
|:-:|:-:|:-:|
| **Fame** | `0` | `32,000` |
| **Karma** | `-32,000` | `32,000` |

## Titles
Fame and karma combine to create a character's title.

| Karma | < 1,250 Fame | < 2,500 Fame | < 5,000 Fame | < 10,000 Fame | >= 10,000 Fame |
|:-:|:-:|:-:|:-:|:-:|:-:|
| >= 10,000 | Trustworthy | Estimable | Great | Glorious | Glorious Lord/Lady |
| >= 5,000 | Honest | Commendable | Famed | Illustrious | Illustrious Lord/Lady |
| >= 2,500 | Good | Honorable | Admirable | Noble | Noble Lord/Lady |
| >= 1,250 | Kind | Respectable | Proper | Eminent | Eminent Lord/Lady |
| >= 625 | Fair | Upstanding | Reputable | Distinguished | Distinguished Lord/Lady |
| 0 +/- 624 | — | Notable | Prominent | Renowned | Lord/Lady |
| <= -625 | Rude | Disreputable | Notorious | Infamous | Dishonored Lord/Lady |
| <= -1,250 | Unsavory | Dishonorable | Ignoble | Sinister | Sinister Lord/Lady |
| <= -2,500  | Scoundrel | Malicious | Vile | Villainous | Dark Lord/Lady |
| <= -5,000 | Despicable | Dastardly | Wicked | Evil | Evil Lord/Lady |
| <= -10,000 | Outcast | Wretched | Nefarious | Dread | Dread Lord/Lady |