---
title: Patch Notes
description: 
published: true
date: 2026-11-18T04:31:22.049Z
tags: 
editor: markdown
dateCreated: 2026-11-04T19:38:55.944Z
---

# Patch Notes
## 2026.11.18
- Add novel [reputation](/Reputation) system mechanics:
	- Fame now offers a choice: `more gold for gems`, or more `skill gain chance`
	- High karma unlocks NPC interaction within `Serpent's Hold`
	- Add teleporter to `Serpent's Hold` from the guard outpost north of `Trinsic`
	- Low karma unlocks NPC interaction within `Buccaneer's Den`
	- Remove moongate access to `Buccaneer's Den`
	- Add `Thugs` and `Templars` at their town's teleporters for karma farming
	- Item donations to NPCs no longer give `fame`
	- Utilize existing `shrine karma unlock` system
- Decriminalize attacking one's own `pet`, to train weapon skills
- `Pets` now appear as allies to their owners
- Add additional `Strongbox`/`Trash Barrel` commands
- Fix `Spyglass` showing `Trammel` moon cycle
## 2026.11.17
- `Veterinary` gives `level / 25` extra tiles to pet bandage range
- `Bandage` weight halved
- `Runebook` use range set to `3` from `2`
- `Runebook` use cooldown set to `3` from `7`
- Remove non-T2A items from `Carpentry` crafting gump
- Set `House Decay` to `90` days
- Disable `House Decay` dropping items, they're deleted instead
- `Meditation`, `Potions`, and `Wrestling` ignore equippable lights
## 2026.11.16
- Adjust `Nightmare` spawn to `1 ~ 2` hours
- Adjust `Silver Steed` spawn to `0.5 ~ 1` hours
## 2026.11.15
- Fix MvM damage (was halved while adjusting MvP damage)
- Move server daily restart to a systemd service
- Adjust various `lockpicking` requirements
- Reduce carry weight of `Gold` and `Reagents` by half
- Marked `Recall Runes` now display custom description
- Fix bug with `Magic Reflect` sometimes failing
- `Potions` are now stackable
- `Gold` will now autosplit when the max stack size is reached
- Allow casting with equippable lights (e.g., `Candle`)
## 2026.11.14
- Add `Stealth Archer` ambush mechanic:
	- Breaking `Hiding` with a `Ranged Weapon` attack causes `1.5×` damage (works while mounted)
	- Breaking `Hiding -> Stealth` with a `Ranged Weapon` attack gets additional bonuses for **every footstep**
	- Each **stealthed footstep** grants `0.05x` damage and `10%` of the missing accuracy required for a guaranteed hit
  - After all `10` stealthed steps, the shot **cannot miss** and does a grand total of `2.0×` damage
  - An ambushed target, successfully or not, cannot be ambushed again **by anybody** for `1` minute
  - The `Hiding` skill **must be used first** for ambushes, neither the spell [Invisibility](/Invisibility) nor [Invisibility Potions](/Invisibility_Potion) suffice
- Fix armor being counted twice (wow)
- Significantly increase monster physical damage to players, ServUO's T2A implementation was very wrong
- Fix NPC trainers not recognizing `"Discordance"` term, the old term was `"Enticement"`
## 2026.11.13
- Enable Town, Seeker, and Prisoner `escort quests`
- Adjust `Lost Lands` spawners, particularly `Frenzied Ostards`
- Remove `Seed` drop sources
- Rebalance `MageAI`, creatures with higher `Magery` will now cast spells more often, those with lower will cast less often
## 2026.11.12
- Add [shiny mechanic](/Items/Mounts) to `Silver Steeds` and `Nightmares`
- Revert follower slot change (e.g., `Dragons` take `3` slots again)
- Block `Recall`, `Mark`, and `Gate Travel` to/from/in `The Lost Lands`
- Remove `Fire Steeds`, `Acid Elementals` from spawners
## 2026.11.11
- Remove `Fire Horn` drop sources
- Refactor `Treasure Map` loot, allow cascading
- Pets now respond to their custom names properly (e.g., `a` won't trigger `aa`)
- Disable "Virtue Dungeon Armor" rewards
- Disable seasonal events
- Reduce `Blood Elemental` spawn count in `Shame`
- Fully disable `Bulk Order` system
- Disable all quests except the `Grizelda` quest
## 2026.11.10
- All pets now take up `1` follower slot (each character has `5` total)
## 2026.11.09
- Pets given the `follow` command now properly ignore enemies
- `Peacemaking` now has a `10s` cooldown on success and `5s` on fail
- The server will now automatically restart once per day at `12 GMT`
- Removed both NPCs in the Bard's Guild that started mastery quests
## 2026.11.08
- Remove scaling `Discordance` cooldown, it is now always `5` seconds
- Add `[TimePlayed` command as guildmasters ask for a certain amount of play time
- Fix healthbar gumps going blank when monster is off screen
- Further disable monsters casting `Invisibility`
## 2026.11.07
- Monsters:
  - Now have shorter aggro range
  - No longer path around obstacles
- `Provocation`:
  - Increase duration from `30` seconds to `60`
  - Remove random chance for provoked monsters to break free
- Double `Animal Taming` skill gain speed
- Locked-down `Runebooks` may now be used by anyone
- Added teleporters to access `Cyclops Valley` from the south
## 2026.11.06
- Player corpses now correctly make `bones` indicating 50% duration remaining
- Adjust player corpse decay rate to `60 minutes` total
- Monsters with `Magery`:
	- Now only `Teleport` when stuck
	- No longer cast `Invisibility`
## 2026.11.05b
- Fix `Cartography` crafting gump:
	- Remove `Tattered Wall Maps` & `Wall Map of Eodon`
  - Move `Star Chart` from last to first
- Allow ore smelting directly from pack animal inventory
- Pet follow speed now correctly matches player speed
- Remove `Crafting Resources` and `Special Scrolls` drops from `Treasure Maps`
- Fleeing monsters will now walk instead of run
## 2026.11.05a
- Fix random `Scroll` drops all being low level
- Remove `Special Resources` drop from `Treasure Maps`
- `Magic Reflect`, `Reactive Armor`, and `Protect` should properly stack
## 2026.11.04
- Remove `Necromancer Scroll` drops from 15 additional monsters
- Disable random `Necro Reagent` drops from all monsters
- Change `[password` command to work without a GM present
- Allow `Protect`, `Reactive Armor`, and `Magic Reflect` to work simultaneously
- Add map level to name of completed `Treasure Maps`
## 2026.11.03
These are changes to ServUO's base. This is the server's starting point.
- ServUO gate set to T2A
	- This disables a ton of content that wont be listed here
- Stat cap set to 100
- Champions disabled
- Programs other than Razor disabled
- Factions disabled
- Duel Arenas enabled
- Guild PvP enabled
- Map geography set to Felucca only
- Map PvP & shove rules set to Trammel
- New Haven disabled as starting city
- Moongates changed to Felucca only
- Creature bonding disabled
- Swing cycle modified to T2A-esque
- Provocation cooldown changed to 5 seconds
- Provocation can target the bard who used it
- Moonglow zoo spawns changed to avoid guard aggro
- Council of Mages moved to proper location
- Recall enabled to and from T2A
- Necromancer scroll random drops disabled
- Necro scrolls drops from Imps disabled (others exist)
- Instruments no longer drop with modifiers
- Boats can be drydocked by clicking Tillerman
- Monster Mage AI has been toned down
- Mounts no longer fatigue when damage is taken
- Magic Reflect has been changed to its old form
- Followers move faster
- Reagent vendors have higher stocks
- Mage vendors sell Recall & Mark scrolls
- Boat decay is 1 day
- House decay is 7 years