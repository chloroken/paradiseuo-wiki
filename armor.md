# Armor
Armor reduces incoming physical damage. Heavy armor lowers stamina and Dexterity, and most armor slows mana regeneration, even with [Meditation](/meditation). Leather armor doesn't slow it at all, studded armor slows it half as much, and shields count too. Bone armor is never crafted and is only found as loot. Armor and shields of [colored metal](#metal-types) also ward off spells.

## How Armor Works
When hit by an attack, the following happens in order:
1. Characters with Parrying who fight without magic reduce incoming damage through [Valor](/valor).
1. The defender tries to [block with a shield](/parrying). A successful block reduces the damage.
1. A random piece of the defender's armor is hit (see the table below), and it reduces the damage by a percentage.
1. Arch Protection and an equipped shield reduce the damage by a further flat amount. See below.
1. The damage is dealt.

Each piece of armor reduces damage by a random `1%` to `2%` for every point of its armor rating, up to `90%`. A plate chest with `40` armor reduces damage by `40%` to `80%`. Because the reduction is a percentage, armor protects against hard hits as well as light ones.

Arch Protection and an equipped shield then remove a flat amount, between `50%` and `100%` of `(Arch Protection + 2 * Shield Rating) * Flat Scale`, using the scale for the body slot that was hit. For a heater shield at `100` Parrying, that's up to `8` damage on a chest hit and `1` on a hand hit.

| Body Slot | Chance to Be Hit (%) | Flat Scale (%) |
|:-|:-:|:-:|
| Neck | 7 | 7 |
| Hands | 7 | 7 |
| Arms | 14 | 15 |
| Head | 15 | 14 |
| Legs | 22 | 22 |
| Chest | 35 | 35 |

## Durability
When a piece of armor is hit, it loses durability, and blunt weapons cause more durability loss. Armor that runs out of durability breaks and must be repaired. Each time a piece of armor breaks, its maximum durability decreases. Eventually it can no longer be repaired, and it vanishes the next time it breaks. Metal armor can be [repaired](/blacksmithing#repairing) by a blacksmith, but leather, studded, and bone armor can't be repaired at all.

## Metal Types
Ringmail, chainmail, plate, and shields forged by a [blacksmith](/blacksmithing#metal-types) can be made of colored metal instead of iron. Colored metal adds no armor rating. Instead, it reduces damage from spells, including the necromancy of the [Lich King](/lich_king) and the flames of Fire Field, by more for rarer metals.

| Metal | Spell Damage Reduction<br>for a Full Set (%) | Share of Colored<br>Loot Armor (%) |
|:-|:-:|:-:|
| Dull copper | 1.25 | 22.2 |
| Shadow iron | 2.5 | 19.4 |
| Copper | 3.75 | 16.7 |
| Bronze | 5 | 13.9 |
| Gold | 6.25 | 11.1 |
| Agapite | 7.5 | 8.3 |
| Verite | 8.75 | 5.6 |
| Valorite | 10 | 2.8 |

A full set is armor in every body slot plus a shield. Each piece adds its share of the reduction, out of `135` parts: `35` each for the chest and the shield, `22` for the legs, `15` for the arms, `14` for the head, and `7` each for the neck and hands. A full valorite suit without a shield reduces spell damage by about `7.4%`, and pieces of different metals add up on their own.

`10%` of the ringmail, chainmail, plate, and shields that monsters drop come in a colored metal, matching the rarity of [ore veins](/mining#ore-and-veins). Colored metal can stack with magic properties or exceptional quality, and [Arms Lore](/arms_lore#examining) can judge how well a piece wards off magic. Weapons never drop in colored metal.

