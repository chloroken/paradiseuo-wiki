# Crafting
Crafters turn gathered resources into weapons, armor, clothing, furniture, potions, scrolls, and more. Each crafting skill needs its own tool, which opens a menu of everything that skill can make. Items with their own pages are listed on [Items](/items).

## Crafting Skills
| Skill | Tool | Main Resources | Makes |
|:-|:-:|:-:|:-:|
| [Alchemy](/alchemy) | Mortar and pestle | Reagents, empty bottles | Potions |
| [Blacksmithing](/blacksmithing) | Smith's hammer or tongs | Ingots | Metal weapons and armor |
| [Carpentry](/carpentry) | Saw and other woodworking tools | Boards, logs | Furniture, containers, wooden weapons |
| [Cartography](/cartography) | Mapmaker's pen | Blank maps or blank scrolls | Maps |
| [Cooking](/cooking) | Skillet, rolling pin, and others | Food ingredients | Food |
| [Fletching](/fletching) | Fletcher's tools | Boards, feathers | Bows, crossbows, arrows, bolts |
| [Inscription](/inscription) | Scribe's pen | Blank scrolls, reagents | Spell scrolls |
| [Tailoring](/tailoring) | Sewing kit | Cloth, leather | Clothing, leather armor |
| [Tinkering](/tinkering) | Tinker's tools | Ingots, boards | Tools, jewelry, traps |

Blacksmithing needs an anvil and a forge nearby. Raw resources come from the gathering skills: [Mining](/mining) for ore, [Lumberjacking](/lumberjacking) for logs, and [Fishing](/fishing) for fish to cook. Ore can be smelted straight from a pack animal's backpack.

## Success Chance
Every item has a minimum and a maximum skill. Below the minimum it can't be made, and at the maximum it never fails. In between, the chance rises evenly from a starting chance at the minimum:

| Starting Chance (%) | Skills |
|:-|:-:|
| 0 | Alchemy, Blacksmithing, Cartography, Cooking, Inscription, Tinkering |
| 50 | Carpentry, Fletching, Tailoring |

Every attempt, success or failure, has a chance to raise the crafting skill, as long as the crafter's skill is between the item's minimum and maximum. A failed attempt can use up some of the resources.

## Exceptional Items
Weapons, armor, clothing, furniture, and other gear can come out exceptional. Every other crafted item is regular quality. Exceptional quality is a modifier, like the magic properties found on loot, and a weapon can't have both. See [Magic Weapons: Modifiers](/magic_weapons#modifiers).

An exceptional item gets these bonuses:
- Weapons do `20%` more damage. The extra damage is flat, so critical strikes, ambushes, and bonks don't multiply it. See [Combat: Damage](/combat#damage).
- Armor gets `8` more armor rating. See [Armor](/armor).
- Weapons and armor last `20%` longer before breaking.

The chance of a crafted item becoming exceptional depends on the success chance and the crafter's skill:

| Skill | Exceptional Chance at<br>Full Success Chance (%) |
|:-|:-:|
| Up to 95 | 40 |
| 97 | 46 |
| 99 | 52 |
| 100 | 55 |

Fletching works differently: half the success chance, minus `10%`, so at most `40%`.

### Maker's Mark
A crafter with `100` in the skill can mark exceptional items with their name, which shows as *crafted by* when the item is single-clicked. Blacksmithing, Carpentry, Fletching, Inscription, Tailoring, and Tinkering can mark items. The `Mark Item` button in the crafting menu chooses whether to always mark, never mark, or ask each time.