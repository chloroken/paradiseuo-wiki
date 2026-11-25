---
title: Weapon Effects
description: Critical strikes, sapping vigor, Concussion, Crushing, and Paralyzing Blows, the shillelagh, and stun
published: true
date: 2026-11-25T12:12:47.332Z
tags: 
editor: markdown
dateCreated: 2026-11-24T03:38:58.666Z
---

# Weapon Effects
Most weapon types have a weapon effect, which can trigger when a hit lands. Weapon effects are for players only. Monsters, hirelings, and other NPCs never trigger them, even with the same weapons. Some effects also only work against monsters.

Unless noted, each weapon effect is controlled by [Arms Lore](/arms_lore), from nothing at `0` to full strength at `100`. A character without Arms Lore can use any weapon, but never lands its effect. Which weapons have which effect is listed on [Weapons](/weapons#weapon-types).

| Name | Effect |Weapons | Trigger | Works Against |
|:-|:-:|:-:|:-:|:-:|
| [Critical strikes](#critical-strikes) | 2x damage | Swords | Each sword's own chance, scaled by Arms Lore | Anything |
| [Sapping vigor](#sapping-vigor) | Reduces enemy damage | One-handed maces | Every hit, amount scaled by Arms Lore | Monsters |
| [Concussion Blow](#concussion-blow) | Reduces enemy Intelligence | Polearms | Anatomy / 400, no Arms Lore needed | Anything |
| [Crushing Blow](#crushing-blow) | Reduce enemy attack speed | Two-handed maces, staves | Arms Lore / 400 | Monsters |
| Crushing Blow (secondary effect) | Splash damage hits everything within a tile | Two-handed maces | Blacksmithing / 100 | Monsters |
| [Paralyzing Blow](#paralyzing-blow) | Freezes enemy | Pitchforks, short spears, spears | Arms Lore / 400 | Anything |
| [Shillelagh](#shillelagh) | 10x damage, 9s cooldown | Shepherd's crook | First hit after a 9 second cooldown, no Arms Lore needed | Anything |
| [Stun](#stun) | Freezes enemy | Fists | (Wrestling + Anatomy) / 400, no Arms Lore needed | Anything |

Crushing Blow and Paralyzing Blow each land on `Arms Lore / 400` of hits with the right weapon, which is `25%` at `100` Arms Lore. Four effects don't use Arms Lore: Concussion Blow uses [Anatomy](/anatomy), Crushing Blow's secondary effect uses [Blacksmithing](/blacksmithing), the shillelagh scales with [Herding](/herding), and stun needs Wrestling and Anatomy. [Crossbow volleys](/archery#crossbow-volley), [poison](/poisoning), and [ambushes](/ambush) aren't weapon effects, so Arms Lore doesn't change them either.

## Critical Strikes
Swords can land a critical strike, which doubles the hit's damage before armor, including a magic weapon's damage bonus. Each sword has its own chance, scaled by Arms Lore, so `50` Arms Lore gives half the chance shown below. The chances are set so every sword does about the same damage over time, and the slowest swords hit in the biggest bursts.

| Sword | Critical Strike Chance (%)<br>at 100 Arms Lore |
|:-|:-:|
| Katana | 12 |
| Broadsword | 10 |
| Scimitar | 15 |
| Cutlass | 17 |
| Longsword | 26 |
| Viking sword | 40 |

Only swords land critical strikes, not axes, polearms, or knives. The attacker sees *You land a critical strike!* in their journal.

## Sapping Vigor
One-handed maces sap a monster's vigor. Each hit saps vigor equal to the damage dealt, scaled by Arms Lore, so `50` Arms Lore saps half as much and a character without Arms Lore saps none. The monster's melee attacks hit as if its Strength were that much lower, down to half its normal Strength. Its health isn't affected. The sap wears off `30` seconds after the last one-handed mace hit from anyone.

The attacker sees *\*saps vigor\** over their head when a sap starts, and everyone nearby sees *\*looks drained of vigor\** when the monster is fully drained. Vigor can only be sapped from monsters.

## Concussion Blow
Polearms can land a Concussion Blow on `Anatomy / 400` of hits, `25%` at `100` Anatomy. It halves the target's Intelligence and lowers its maximum mana for `30` seconds, and doesn't stack. It's aimed at the head, so it uses Anatomy instead of Arms Lore. Two-handed axes don't land it.

Everyone nearby sees *\*looks concussed\** over the target.

## Crushing Blow
Two-handed maces and staves can land a Crushing Blow, which makes the target attack at half speed for `10` seconds. Another Crushing Blow restarts the time instead of stacking. The shepherd's crook is the exception and never lands one.

Crushing Blow only works against monsters. Everyone nearby sees *\*looks dazed\** over the target.

With a two-handed mace, each Crushing Blow has a `Blacksmithing / 100` chance to splash, every time at grandmaster [Blacksmithing](/blacksmithing). Every creature within `1` tile of the target takes the same hit, each reduced by its own armor. Since the splash needs a Crushing Blow first, it needs Arms Lore too. The splash only does damage, with no slow, and gives no skill gains. Staves never splash.

The splash only hits creatures that are fair game: monsters and the creatures they summon. It never hits players, pets, summons, hirelings, or anything innocent, such as townsfolk and animals.

## Paralyzing Blow
Spears, short spears, and pitchforks can land a Paralyzing Blow, which freezes the target in place for `2` seconds.

Everyone nearby sees *\*looks stuck\** over the target.

## Shillelagh
In the hands of a herder, a shepherd's crook becomes a shillelagh. This magical stick gets an extended attack range by `1` tile every `33.3` levels of Herding for a capstone bonused max range of `4`.

The first crook hit that lands after a `7` second cooldown is a "bonk" and consumes `25%` of the attacker's current mana and never misses. The crook's damage is multiplied by `consumed mana * 2 / (10 - floor(herding / 20))` maxing out at `10×` while max Herding and with the maximum mana consumption of `25`. When the cooldown ends, the attacker sees *Your crook hums* in their journal, sees a glowing effect on their character, and hears a sound effect.

| Mana Consumed | Bonk Damage |
|:-|:-:|
| 5 mana | 1× |
| 25 mana | 5× |
| 50 mana | 10× |

- The multiplier applies to the crook's damage roll, before Tactics, Strength, and Anatomy.
- A [magic](/magic_weapons) crook's damage bonus is not multiplied by bonk, it's just added normally.
- Otherwise a bonk is a normal hit. Armor and shields reduce its damage.
- The cooldown belongs to the player, so switching crooks doesn't reset it.

## Stun
Fighting with empty hands allows one move, Stun, which freezes the target in place for `4` seconds. It's attempted automatically when a punch hits, and needs `80` Wrestling and `80` Anatomy, but no Arms Lore. See [Wrestling: Wrestling Moves](/wrestling#wrestling-moves).