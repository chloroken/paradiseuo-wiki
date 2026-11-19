# Treasure Map
Treasure maps drop from monsters and have a level from `0` to `5`, with stronger monsters dropping higher-level maps. Level `0` maps only drop for Young players.

A map must be decoded with [Cartography](/cartography) before the location it shows can be found in the world. The treasure chest must then be dug up with a shovel (made easier with [Mining](/mining)), unlocked with [Lockpicking](/lockpicking), and its trap disarmed with [Magery](/magery) or [Remove Trap](/remove_trap). Finally, the guardian monsters must be defeated. Only then does the treasure chest become vulnerable.

Monsters keep spawning while the chest is looted. The type of monsters that spawn depends on the chest's level.

## Decoding
Double-click a treasure map to try decoding it.

| Map Level | Minimum Cartography | Guaranteed Cartography | Gain Limit |
|:-|:-:|:-:|:-:|
| 0 | 0 | 0 | 0 |
| 1 | 0 | 0 | 30 |
| 2 | 50 | 60 | 90 |
| 3 | 65 | 75 | Never |
| 4 | 80 | 90 | Never |
| 5 | 90 | 100 | Never |

## Lockpicking
A lockpicker can use a [lockpick](/lockpick) on a treasure chest to try opening it.

## Disarming
A treasure chest can be disarmed from range with [Telekinesis](/telekinesis), avoiding the explosion and its damage. Without Magery, the only options are Remove Trap or taking the trap damage.

## Loot
A treasure chest's loot depends on its map level. Treasure maps found inside are always one level lower.

| Chance (%) | Drop | Amount |
|:-|:-:|:-:|
| 100 | Gold | 5,000 * Level |
| 100 | Reagents | (40 to 60) * (Level + 1) |
| 100 | Gems | 3 * Level + 1 |
| 100 | Magic equipment | 6 * Level |
| 100 | Scrolls | 5 * Level |
| 50 | Treasure map | 1 |
| 1 | [Skeleton key](/skeleton_key) | 1 |
