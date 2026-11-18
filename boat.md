---
title: Boat
description: 
published: true
date: 2026-11-18T22:45:16.211Z
tags: 
editor: markdown
dateCreated: 2026-11-17T22:49:31.290Z
---

# Boat
Boats allow travel by sea and river. They are bought from shipwrights near docks. **Boats sink `24` hours after its last refresh**, which is unusual for Ultima Online.

## Ships
| Ship | Price | Hold (stones) |
|:-|:-:|:-:|
| Small Ship | 10,177 | 400 |
| Small Dragon Ship | 10,177 | 400 |
| Medium Ship | 11,552 | 400 |
| Medium Dragon Ship | 11,552 | 400 |
| Large Ship | 12,927 | 400 |
| Large Dragon Ship | 12,927 | 400 |

A dragon ship differs from the ship of the same size only in its look. Shipwrights also sell a spyglass for `3` gold, a flavor item that shows the moon's current phase.

## Launching and Keys
Double-click a ship deed and target open water to launch the ship. Two ship keys are created: one goes into the owner's backpack and one into their bank box. The keys lock and unlock the ship's planks on each side, which are double-clicked to board. Keep the bank key safe, because anyone holding a key can dry-dock the ship, stealing it.

## Manual Navigation
Anyone standing on the boat can give commands to the tillerman.

| Command | Effect |
|:-|:-:|
| `Forward` / `Unfurl sail` | Sail forward at full speed |
| `Back` | Sail backward |
| `Left` / `Right` | Drift sideways to port / starboard |
| `Forward left` / `Forward right` | Sail diagonally forward |
| `Back left` / `Back right` | Sail diagonally backward |
| `Slow forward`, `Slow left`, etc. | Any of the above at half speed |
| `Forward one`, `Left one`, etc. | Move a single tile in that direction |
| `Turn right` / `Starboard` | Turn the boat 90° right |
| `Turn left` / `Port` | Turn the boat 90° left |
| `Come about` | Turn the boat 180° |
| `Stop` / `Furl sail` | Stop moving |

- At full speed, a ship moves forward `4` tiles per second. Sideways and backward movement is half that, and slow commands halve it again.
- A ship stops when it reaches land, another ship, or any other obstacle. The tillerman says *Ar, we've stopped sir.*
- Turning needs enough open water around the ship. If there isn't room, the tillerman says *Ar, can't turn sir.*
- Sailing off the edge of the world brings the ship out on the opposite edge.

## Automatic Navigation
A ship can follow a course plotted on a map.

1. Put a map in the backpack and double-click it. Sea charts and world maps work best. Treasure maps can't be plotted on.
1. Click `Plot Course`, then click on the map to place pins. Pins are numbered in the order they're placed and can be dragged to move them. `Clear Course` removes them all.
1. Board the ship and drop the map on the tillerman. He says *A map!* and the course is set.
1. Give a course command:

| Command | Effect |
|:-|:-:|
| `Start` | Sail the whole course from the first pin |
| `Continue` | Resume the course from where it stopped |
| `Goto #` | Sail the course to pin # |
| `Single #` | Sail straight to pin # and stop |
| `Nav` | Ask which pin the ship is heading to |

The ship sails each leg at full speed and turns on its own. If land or another obstacle is in the way, it stops. Place pins over open water, and say `Continue` to resume after steering around a blockage by hand. Courses only work in Felucca and Trammel.

The map isn't used up. The tillerman hands it back, and the same map can be given to any number of ships. The course stays on the ship through dry-docking and server restarts until a new map is given. If the pins change, give the map to the tillerman again.

## The Hold
The hold is the container at the front of the ship and carries up to `400` stones. Items can also be dropped on the deck, and they move with the ship.

## Dry-Docking
To store a ship, step off it and double-click the tillerman with a ship key in the backpack. Before dry-docking, the ship must be empty, the deck clear of items, and nobody can be aboard.

Dry-docking is free and instant. The ship becomes a toy ship in the backpack, and its keys are removed. Double-click the model to launch the ship again with a fresh set of keys. A dry-docked ship in toy form never decays.

## Decay
A ship sinks `24` hours after it was last refreshed. A ship is refreshed at every world save while a player is aboard, and it never decays while someone is aboard or while it's moving.

**When a ship sinks, everything in the hold and on deck is lost.** Dry-dock ships that won't be used for a while.

Boat decay is short because players traditionally used rows of boats to block objectives, or even entire islands. A shorter decay makes this much more tedious.

## Naming
| Command | Effect | Permission |
|:-|:-:|:-:|
| `Set name <name>` | Rename the ship | Owner |
| `Remove name` | Clear the ship's name | Owner |

The owner can also rename the ship by double-clicking the tillerman while aboard. Other characters on the owner's account can't rename the ship.
