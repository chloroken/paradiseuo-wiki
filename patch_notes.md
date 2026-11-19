---
title: Patch Notes
description: 
published: true
date: 2026-11-19T05:15:35.384Z
tags: 
editor: markdown
dateCreated: 2026-11-04T19:38:55.944Z
---

# Patch Notes
Changes to *Paradise*, newest first.

## 2026.11.19
- Add the [Antimage](/features#antimage) rework, so characters with less Magery fight better:
    - Tactics adds up to `30` points of weapon skill when rolling to hit
    - Physical damage taken is reduced by up to `20%`
    - Hit points regenerate up to `5×` faster
    - All three bonuses are full at `0` Magery and shrink to nothing at `100`
    - Only players get the bonuses
- Tie Antimage toughness to Parrying and regeneration to Anatomy, scaled against Magery like accuracy from Tactics
- Fix [Young players](/young_player) being unable to Recall, Gate Travel, or use moongates
- Wrestling moves are now automatic:
    - Armed players and human NPCs are disarmed, and everything else is stunned
    - Moves are only attempted when a punch hits, and need free hands
    - Moves no longer cost stamina
    - Any attempt starts a `10` second cooldown
    - The stun and disarm buttons now only explain that the moves are automatic
- Dexterity now adds `1.75` stones of carrying capacity per point, half as much as Strength
- Thrown weapons can no longer be equipped
- Fix Mana Drain and Mana Vampire being resisted almost every time
- Remove monsters added after T2A from the world, including plague beasts, boglings, bog things, toxic elementals, juka, golems, greater dragons, and shadow wyrms
- Close the dungeons added after T2A: Sanctuary, Prism of Light, Blighted Grove, Painted Caves, and Khaldun
- Remove leftover teleporters to Ter Mur, the Stygian Abyss, and the champion spawn network

## 2026.11.18
- Add new [reputation](/reputation) mechanics:
    - Fame now offers a choice: more gold for gems, or a higher chance of skill gain
    - High Karma unlocks NPC services in Serpent's Hold
    - Add a teleporter to Serpent's Hold from the guard outpost north of Trinsic
    - Low Karma unlocks NPC services in Buccaneer's Den
    - Remove moongate access to Buccaneer's Den
    - Add thugs and templars at their towns' teleporters for Karma farming
    - Item donations to NPCs no longer give Fame
    - Speak a shrine's mantra beside its ankh to unlock locked Karma
- Attacking one's own [pet](/pet) is no longer criminal, so pets can be used to train weapon skills
- Pets now appear as allies to their owners
- Add more strongbox and trash barrel commands
- Fix the spyglass showing Trammel's moon phase
- Fighting one's own pets no longer blocks Recall and Gate Travel
- Saying `claim` at a stable now opens the list of stabled pets
- The stealth archer's *You are in perfect position!* message now only appears once

## 2026.11.17
- [Veterinary](/veterinary) adds `Veterinary / 25` extra tiles to pet bandage range
- Bandage weight halved
- Runebook use range set to `3`, from `2`
- Runebook use cooldown set to `3` seconds, from `7`
- Remove non-T2A items from the Carpentry crafting menu
- Set house decay to `90` days
- House decay no longer drops items; they're deleted instead
- Meditation, potions, and Wrestling ignore equippable lights

## 2026.11.16
- Adjust nightmare spawn time to `1` to `2` hours
- Adjust silver steed spawn time to `0.5` to `1` hours

## 2026.11.15
- Fix MvM damage (it was halved while adjusting MvP damage)
- Move the server's daily restart to a scheduled cron job
- Adjust various Lockpicking requirements
- Halve the weight of gold and reagents
- Marked recall runes now show a custom description
- Fix a bug with Magic Reflection sometimes failing
- Potions are now stackable
- Gold now splits automatically when a stack reaches its maximum size
- Allow casting with equippable lights, such as candles

## 2026.11.14
- Add the stealth archer ambush mechanic:
    - Breaking Hiding with a ranged weapon attack does `1.5×` damage (works while mounted)
    - Breaking Hiding, then Stealth, with a ranged weapon attack gives extra bonuses for every footstep
    - Each stealthed footstep adds `0.05×` damage and `10%` of the missing accuracy needed for a guaranteed hit
    - After all `10` stealthed steps, the shot can't miss and does a total of `2.0×` damage
    - An ambushed target, successful or not, can't be ambushed again by anybody for `1` minute
    - The Hiding skill must be used for ambushes; neither the [Invisibility](/invisibility) spell nor [invisibility potions](/invisibility_potion) work
- Fix armor being counted twice (wow)
- Significantly increase monster physical damage to players, since ServUO's T2A implementation was very wrong
- Fix NPC trainers not recognizing the term `Discordance` (the old term was `Enticement`)

## 2026.11.13
- Enable town, seeker, and prisoner escort quests
- Adjust Lost Lands spawners, particularly frenzied ostards
- Remove seed drop sources
- Rebalance MageAI: creatures with higher Magery now cast spells more often, and those with lower Magery cast less often

## 2026.11.12
- Add the [Shiny](/mount) mechanic to silver steeds and nightmares
- Revert the follower slot change (for example, dragons take `3` slots again)
- Block Recall, Mark, and Gate Travel to, from, and within the Lost Lands
- Remove fire steeds and acid elementals from spawners

## 2026.11.11
- Remove fire horn drop sources
- Refactor treasure map loot, and allow cascading
- Pets now respond to their custom names properly (for example, `a` won't trigger `aa`)
- Disable Virtue Dungeon Armor rewards
- Disable seasonal events
- Reduce the blood elemental spawn count in Shame
- Fully disable the Bulk Order system
- Disable all quests except Grizelda's quest

## 2026.11.10
- All pets now take up `1` follower slot (each character has `5` in total)

## 2026.11.09
- Pets given the `follow` command now properly ignore enemies
- Peacemaking now has a `10` second cooldown on success and `5` seconds on failure
- The server now restarts automatically once a day at `12:00` GMT
- Remove both NPCs in the Bard's Guild that started mastery quests

## 2026.11.08
- Remove the scaling Discordance cooldown; it is now always `5` seconds
- Add the `[TimePlayed` command, since guildmasters ask for a certain amount of play time
- Fix health bar gumps going blank when a monster is off screen
- Further stop monsters casting Invisibility

## 2026.11.07
- Monsters:
    - Now have a shorter aggro range
    - No longer path around obstacles
- Provocation:
    - Increase duration from `30` seconds to `60`
    - Remove the random chance for provoked monsters to break free
- Double Animal Taming skill gain speed
- Locked-down runebooks can now be used by anyone
- Add teleporters to reach Cyclops Valley from the south

## 2026.11.06
- Player corpses now correctly turn to bones at `50%` of their duration
- Adjust player corpse decay to `60` minutes in total
- Monsters with Magery:
    - Now only cast Teleport when stuck
    - No longer cast Invisibility

## 2026.11.05b
- Fix the Cartography crafting menu:
    - Remove tattered wall maps and the wall map of Eodon
    - Move the star chart from last to first
- Allow smelting ore directly from a pack animal's inventory
- Pet follow speed now correctly matches player speed
- Remove crafting resource and special scroll drops from treasure maps
- Fleeing monsters now walk instead of running

## 2026.11.05a
- Fix random scroll drops all being low level
- Remove special resource drops from treasure maps
- Magic Reflection, Reactive Armor, and Protection should properly stack

## 2026.11.04
- Remove necromancer scroll drops from `15` additional monsters
- Disable random necromancer reagent drops from all monsters
- Change the `[password` command to work without a GM present
- Allow Protection, Reactive Armor, and Magic Reflection to work at the same time
- Add the map level to the name of completed treasure maps

## 2026.11.03
These are the changes to ServUO's base, and the server's starting point.
- ServUO's era set to T2A, which disables a lot of content not listed here
- Stat cap set to `100`
- Champions disabled
- Programs other than Razor disabled
- Factions disabled
- Duel arenas enabled
- Guild PvP enabled
- Map geography set to Felucca only
- Map PvP and shove rules set to Trammel
- New Haven disabled as a starting city
- Moongates changed to Felucca only
- Creature bonding disabled
- Swing cycle changed to be more like T2A
- Provocation cooldown changed to `5` seconds
- Provocation can target the bard who used it
- Moonglow Zoo spawns changed to avoid guard aggro
- Council of Mages moved to its proper location
- Recall enabled to and from T2A
- Necromancer scroll random drops disabled
- Necromancer scroll drops from imps disabled (others exist)
- Instruments no longer drop with modifiers
- Boats can be dry-docked by clicking the tillerman
- Monster mage AI toned down
- Mounts no longer tire when damage is taken
- Magic Reflection changed to its old form
- Followers move faster
- Reagent vendors have larger stocks
- Mage vendors sell Recall and Mark scrolls
- Boat decay is `1` day
- House decay is `7` years