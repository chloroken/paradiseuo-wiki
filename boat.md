# Boat
Boats allow travel by sea and river. They are bought from shipwrights near docks, and [sink quickly](#decay) if left unused.

## Ships
| Ship | Price (gold) | Hold (stones) |
|:-|:-:|:-:|
| Small ship | 10,177 | 400 |
| Small dragon ship | 10,177 | 400 |
| Medium ship | 11,552 | 400 |
| Medium dragon ship | 11,552 | 400 |
| Large ship | 12,927 | 400 |
| Large dragon ship | 12,927 | 400 |

A dragon ship differs from the ship of the same size only in its look. Shipwrights also sell a spyglass for `3` gold, a flavor item that shows the moon's current phase.

## Launching and Keys
Double-clicking a ship deed and targeting open water launches the ship. Two ship keys are created: one goes into the owner's backpack and one into their bank box. The keys lock and unlock the ship's planks on each side, which are double-clicked to board. The bank key should be kept safe, because anyone holding a key can dry-dock the ship, stealing it. If the bank box is full, the bank key is lost, so the owner should make room before launching. If the backpack is full, its key drops to the ground.

## Manual Navigation
Anyone standing on the boat can give commands to the tillerman.

| Command | Effect |
|:-|:-:|
| `forward` / `unfurl sail` | Sails forward at full speed |
| `back` | Sails backward |
| `left` / `right` | Drifts sideways to port / starboard |
| `forward left` / `forward right` | Sails diagonally forward |
| `back left` / `back right` | Sails diagonally backward |
| `slow forward`, `slow left`, etc. | Any of the above at half speed |
| `forward one`, `left one`, etc. | Moves a single tile in that direction |
| `turn right` / `starboard` | Turns the boat 90° right |
| `turn left` / `port` | Turns the boat 90° left |
| `come about` | Turns the boat 180° |
| `stop` / `furl sail` | Stops moving |

- At full speed, a ship moves forward `4` tiles per second. Sideways and backward movement is half that, and slow commands halve it again.
- A ship stops when it reaches land, another ship, or any other obstacle. The tillerman says *Ar, we've stopped sir.*
- Turning needs enough open water around the ship. If there isn't room, the tillerman says *Ar, can't turn sir.*
- Sailing off the edge of the world brings the ship out on the opposite edge.

## Automatic Navigation
A ship can follow a course plotted on a map.

1. The navigator puts a map in the backpack and double-clicks it. Sea charts and world maps work best. Treasure maps can't be plotted on.
1. Clicking `Plot Course`, then clicking on the map, places pins. Pins are numbered in the order they're placed and can be dragged to move them. `Clear Course` removes them all.
1. The navigator boards the ship and drops the map on the tillerman. He says *A map!* and the course is set.
1. A course command sets the ship sailing:

| Command | Effect |
|:-|:-:|
| `start` | Sails the whole course from the first pin |
| `continue` | Resumes the course from where it stopped |
| `goto #` | Sails the course to pin # |
| `single #` | Sails straight to pin # and stops |
| `nav` | Asks which pin the ship is heading to |

The ship sails each leg at full speed and turns on its own. If land or another obstacle is in the way, it stops. Pins work best over open water, and saying `continue` resumes the course after steering around a blockage by hand. Courses only work on the Felucca map.

The map isn't used up. The tillerman hands it back, and the same map can be given to any number of ships. The course stays on the ship through dry-docking and server restarts until a new map is given. If the pins change, the map has to be given to the tillerman again.

## The Hold
The hold is the container at the front of the ship and carries up to `400` stones. Items can also be dropped on the deck, and they move with the ship.

## Dry-Docking
To store a ship, the owner steps off it and double-clicks the tillerman with a ship key in the backpack. Before dry-docking, the ship must be empty, the deck clear of items, and nobody can be aboard.

Dry-docking is free, after a confirmation window. The ship becomes a toy ship in its owner's backpack, and its keys are removed. Double-clicking the toy ship launches the ship again with a fresh set of keys. A dry-docked ship in toy form never decays.

## Decay
A ship sinks `24` hours after it was last refreshed. A ship is refreshed at every world save while a player is aboard, and it never decays while someone is aboard or while it's moving.

**When a ship sinks, everything in the hold and on deck is lost.** Ships that won't be used for a while should be dry-docked.

## Naming
| Command | Effect | Permission |
|:-|:-:|:-:|
| `set name <name>` | Renames the ship | Owner |
| `remove name` | Clears the ship's name | Owner |

The owner can also rename the ship by double-clicking the tillerman while aboard. Other characters on the owner's account can't rename the ship.