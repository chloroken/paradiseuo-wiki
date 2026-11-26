# Weapon Effects
Most weapon types have a weapon effect, which can trigger when a hit lands. Weapon effects are for players only. Monsters, hirelings, and other NPCs never trigger them, even with the same weapons. Some effects also only work against monsters.

Weapon effects are largely scaled by [Arms Lore](/arms_lore) in the form of trigger chance, but exceptions exist that are scaled by other skills. A character without Arms Lore can use any weapon, but never lands its effect. Which weapons have which effect is listed on [Weapons](/weapons#weapon-types).

| Name | Effect | Weapons | Trigger | Works Against |
|:-|:-:|:-:|:-:|:-:|
| [Critical strikes](#critical-strikes) | 2× damage | Swords | Each sword's own chance, scaled by Arms Lore | Anything |
| [Sapping vigor](#sapping-vigor) | Reduces enemy damage | One-handed maces | Every hit, amount scaled by Arms Lore | Monsters |
| [Concussion Blow](#concussion-blow) | Reduces enemy Intelligence | Polearms | Anatomy / 400, no Arms Lore needed | Anything |
| [Crushing Blow](#crushing-blow) | Reduces enemy attack speed | Two-handed maces, staves | Arms Lore / 400 | Monsters |
| Crushing Blow (secondary effect) | Splash damage hits everything within a tile | Two-handed maces | Blacksmithing / 100 | Monsters |
| [Paralyzing Blow](#paralyzing-blow) | Freezes enemy | Pitchforks, short spears, spears | Arms Lore / 400 | Anything |
| [Shillelagh](#shillelagh) | Up to 10× damage | Shepherd's crook | First hit after a 7 second cooldown, scaled by Herding and mana, no Arms Lore needed | Anything |
| [Stun](#stun) | Freezes enemy | Fists | (Wrestling + Anatomy) / 400, no Arms Lore needed | Anything |

Crushing Blow and Paralyzing Blow each land on `Arms Lore / 400` of hits with the right weapon, which is `25%` at `100` Arms Lore. Four effects don't use Arms Lore: Concussion Blow uses [Anatomy](/anatomy), Crushing Blow's secondary effect uses Blacksmithing, the shillelagh scales with [Herding](/herding), and stun needs Wrestling and Anatomy. [Crossbow volleys](/archery#crossbow-volley), [poison](/poisoning), and [ambushes](/ambush) aren't weapon effects, so Arms Lore doesn't change them either.

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
With at least `0.1` Herding, the first shepherd's crook hit that lands after a `7` second cooldown is a shillelagh, or bonk. A missed swing doesn't use it up. A bonk reaches `2` tiles, or `3` above `50` Herding, and at `100` Herding it never misses.

A bonk consumes `20%` of the attacker's current mana, up to `20`. The crook's damage roll is then multiplied by `(Mana Consumed / 2) * (Herding / 100)`, so with less mana, the bonk does much less. A bonk reaches its maximum of `10×` with at least `100` mana and `100` Herding. When the cooldown ends, the attacker sees *Your crook hums* in their journal, sees a glowing effect on their character, and hears a sound effect.

| Herding | Mana Consumed | Bonk Damage |
|:-|:-:|:-:|
| 50 | 5 mana | 1.25× |
| 50 | 10 mana | 2.5× |
| 50 | 20 mana | 5× |
| 100 | 5 mana | 2.5× |
| 100 | 10 mana | 5× |
| 100 | 20 mana | 10× |

- The multiplier applies to the crook's damage roll, before Tactics, Strength, and Anatomy.
- A [magic](/magic_weapons) crook's damage bonus is not multiplied by bonk, it's added after.
- Otherwise a bonk is a normal hit. Armor and shields reduce its damage.
- The cooldown belongs to the player, so switching crooks doesn't reset it.

## Stun
Fighting with empty hands allows one move, Stun, which freezes the target in place for `4` seconds. It's attempted automatically when a punch hits, and needs `80` Wrestling and `80` Anatomy, but no Arms Lore. See [Wrestling: Wrestling Moves](/wrestling#wrestling-moves).