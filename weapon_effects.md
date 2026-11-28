---
title: Weapon Effects
description: Critical strikes, blows, the shillelagh, and other effects on hit
published: true
date: 2026-11-28T13:30:00.000Z
tags: 
editor: markdown
dateCreated: 2026-11-26T18:40:29.000Z
---

# Weapon Effects
Most weapon types have a weapon effect, which can trigger when a hit lands. Weapon effects are for players only. Monsters, hirelings, and other NPCs never trigger them, even with the same weapons. Some effects also only work against monsters.

Most weapon effects trigger more often with [Arms Lore](/arms_lore), so a character without it can use any weapon but never lands its effect. A few use other skills instead, as the table shows. Each weapon type's effect is also listed with the [weapon types](/weapons#weapon-types).

| Name | Effect | Weapons | Trigger | Works Against |
|:-|:-:|:-:|:-:|:-:|
| [Critical strikes](#critical-strikes) | 2× damage | Swords | Each sword's own chance, scaled by Arms Lore | Anything |
| [Sapping vigor](#sapping-vigor) | Reduces enemy damage | One-handed maces | Every hit, amount scaled by Arms Lore | Monsters |
| [Concussion Blow](#concussion-blow) | Reduces enemy Intelligence | Polearms | Anatomy / 400, no Arms Lore needed | Anything |
| [Crushing Blow](#crushing-blow) | Reduces enemy attack speed | Two-handed maces, staves | Arms Lore / 400 | Monsters |
| Crushing Blow (secondary effect) | Splash damage hits everything within a tile | Two-handed maces | Blacksmithing / 100 | Monsters |
| Crushing Blow (secondary effect) | Flourish damage hits everything within a tile of the wielder | Black, gnarled, and quarter staves | Carpentry / 100 | Monsters |
| [Paralyzing Blow](#paralyzing-blow) | Freezes enemy | Pitchforks, short spears, spears | Arms Lore / 400 | Anything |
| [Shillelagh](#shillelagh) | Up to 10× damage | Shepherd's crook | First hit after a 7 second cooldown, scaled by Herding, Magery, and mana, no Arms Lore needed | Anything |
| [Stun](#stun) | Freezes enemy | Fists | (Wrestling + Anatomy) / 400, no Arms Lore needed | Anything |

`Arms Lore / 400` is `25%` at `100` Arms Lore. [Crossbow volleys](/archery#crossbow-volley), [poison](/poisoning), and [ambushes](/ambush) aren't weapon effects, so Arms Lore doesn't change them.

## Critical Strikes
Swords can land a critical strike, which doubles the weapon's own damage before armor. A magic or exceptional weapon's [bonus damage](/magic_weapons#modifiers) is added once, not doubled. Each sword has its own chance, scaled by Arms Lore, so `50` Arms Lore gives half the chance shown below. The chances are set so every sword does about the same damage over time, and the slowest swords hit in the biggest bursts.

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

With a two-handed mace, each Crushing Blow has a `Blacksmithing / 100` chance to splash, every time at grandmaster [Blacksmithing](/blacksmithing). Every creature within `1` tile of the target takes the same hit, each reduced by its own armor. Since the splash needs a Crushing Blow first, it needs Arms Lore too. The splash only does damage, with no slow, and gives no skill gains.

With a black, gnarled, or quarter staff, each Crushing Blow instead has a `Carpentry / 100` chance to flourish, every time at grandmaster [Carpentry](/carpentry). Every creature within `1` tile of the wielder takes the same hit, each reduced by its own armor, so a flourish is strongest when surrounded. The main target isn't hit twice. Like the splash, the flourish needs Arms Lore, only does damage, and gives no skill gains.

The splash and the flourish only hit creatures that are fair game: monsters and the creatures they summon. It never hits players, pets, summons, hirelings, or anything innocent, such as townsfolk and animals.

## Paralyzing Blow
Spears, short spears, and pitchforks can land a Paralyzing Blow, which freezes the target in place for `2` seconds.

Everyone nearby sees *\*looks stuck\** over the target.

## Shillelagh
With at least `0.1` Herding, the first shepherd's crook hit after a `7` second cooldown is a shillelagh, or bonk. A bonk never misses. It reaches `2` tiles, or `3` above `50` Herding.

A bonk consumes `20%` of the attacker's current mana, up to `20`. The crook's damage roll is then multiplied by `(Mana Consumed / 2) * (Herding / 100) * (Magery / 100)`, so with less mana, Herding, or Magery, the bonk does much less. It never drops below `1×`, so a bonk always does at least as much as a normal hit. It reaches its maximum of `10×` with at least `100` mana, `100` Herding, and `100` Magery.

Magery counts only base skill, like [Valor](/valor), so the Magery that strengthens a bonk weakens Valor by the same share. When the cooldown ends, an attacker with a crook in hand sees *Your crook hums.* in their journal, sees a glowing effect on their character, and hears a sound effect. A crook in the backpack only hums if a bonk started the cooldown, so fighting with fists or another weapon never sets it off.

| Herding | Magery | Mana Consumed | Bonk Damage |
|:-|:-:|:-:|:-:|
| 100 | 100 | 20 | 10× |
| 100 | 100 | 10 | 5× |
| 100 | 100 | 5 | 2.5× |
| 100 | 50 | 20 | 5× |
| 50 | 100 | 20 | 5× |
| 100 | 0 | 20 | 1× |
| 100 | 100 | 1 | 1× |

- A hit with any other weapon, bare hands included, restarts the cooldown. Spells, missed swings, and equipping a crook don't.
- A character in war mode with empty hands punches anything next to them, and each punch that lands restarts the cooldown. Staying out of reach or switching to peace mode avoids this.
- The multiplier applies to the crook's damage roll, before Tactics, Strength, and Anatomy.
- A magic or exceptional crook's bonus damage isn't multiplied by a bonk. It's added once, after.
- Otherwise a bonk is a normal hit. Armor and shields reduce its damage, and it can raise Mace Fighting.
- The cooldown belongs to the player, so switching crooks doesn't reset it.

## Stun
Fists can [stun](/wrestling#wrestling-moves), freezing the target in place. It's attempted automatically when a punch hits, and depends on Wrestling and Anatomy instead of Arms Lore.