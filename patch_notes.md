---
title: Patch Notes
description: Every change to Paradise, newest first
published: true
date: 2026-11-22T10:10:21.077Z
tags: 
editor: markdown
dateCreated: 2026-11-04T19:38:55.944Z
---

# Patch Notes
Changes to *Paradise*, newest first.

## 2026.11.22
- Move the server to a new VPS
- Adjust Cyclops Valley spawners to be more accurate to T2A
- Add titans, cyclopes, and wyverns to the Lost Lands desert
- Rebalance [pet](/pet#pets-in-combat) combat:
    - Pets' melee hits and spells do `25%` less damage to monsters
    - Monsters' melee hits and spells do `25%` more damage to pets
    - Demibosses' melee hits and spells do double damage to pets
    - A pet's melee hits on another player are halved, the same as a player's
    - A player's summoned creatures count as pets
- Strengthen the [Lich King](/lich_king):
    - Raise his hit points to `9,000` to `11,000`
    - Make him blink to a nearby spot every `5` to `10` seconds in combat, or back to his throne if he strays more than `12` tiles
- Let demibosses path around obstacles
- Stop a second bandage on the same target from restarting one already in progress, so no time or bandages are lost (switching targets still cancels it)

## 2026.11.21
- Add the first demiboss, the [Lich King](/lich_king), in the throne room on floor 3 of [Covetous](/covetous):
    - Built for a group, but a strong player may be able to solo it
    - Casts necromancy spells that players can't use
    - Heals himself now and then in combat, and steadily when no one is in sight
    - Drops a large haul of gold and magic items, `10` high-circle scrolls, a level `5` treasure map, and a guaranteed silver weapon, usually with magic properties
- Add the [liche's ring](/lich_king#liches-ring), which turns a weapon silver but kills its user:
    - Dropped by the Lich King `10%` of the time, and by any lich lord `0.1%` of the time
- Refresh Covetous:
    - Fill floor 1's dead-end hallways with harpies, headless ones, and gazers
    - Add harpies and headless ones to the first mountain pass, and more skeletons to the second
    - Move dread spiders to the back of floor 2's caves, reduce corpsers, and add `2` elder gazers
    - Spread `11` liches across floor 3, and place a lich lord at the stairs to the undead prison and another at the stairs to the dragon cave
- Change silver weapons:
    - Lower the chance of a magic weapon being silver from `5%` to `1%`
    - Make silver the only slayer found on weapons, and remove slayers from looted instruments
    - Give silver weapons a silvery color, and remove the sparkle from slayer hits
- Rework weapons so more of them are worth using:
    - Change the base damage of almost every weapon
    - Give each sword its own critical strike chance, higher for slower swords
    - Make one-handed maces sap a monster's vigor, lowering the damage of its melee hits
    - Move Crushing Blow to two-handed maces and staves, and make it slow the target's attacks instead of doing extra damage
    - Stop maces and staves from draining stamina
    - Make crossbows, but not heavy crossbows, fire up to `3` bolts per shot, each doing `5` to `14` base damage
    - Let knives (butcher knives, cleavers, and skinning knives) be poisoned again
- Change weapon effects:
    - Show messages over the player's head for effects they land, and over the target for effects on it
    - Remove their sounds
    - Show critical strikes and shield blocks in the journal instead of over the player's head
- Show damage numbers over the target when hit
- Draw arrows and bolts from chest height instead of the ground
- Remove newbie protection from starting items and blessing from starting spellbooks, so they drop on death once a character is no longer Young
- Rebalance monsters that hit far harder than others of their strength:
    - Lower lich damage to `10` to `14` and give liches `50` to `60` Wrestling, so they hit less hard but more often
    - Lower ogre lord and arctic ogre lord Strength to `351` to `450`, so they no longer hit harder than dragons
    - Lower frost troll damage to `8` to `14`
    - Lower cyclops damage to `7` to `17`

## 2026.11.20
- Rename Antimage to [Valor](/combat#valor), the warrior's virtue from Ultima lore
- Tune Valor so each bonus comes from a skill, not just by not having Magery:
    - Tactics still passively adds up to `30` points of weapon skill
    - Parrying passively reduces physical damage taken by up to `20%`, before armor reductions
    - Anatomy passively increases hit point regeneration by up to `5×`
    - Each bonus is full at `100` in its skill and `0` Magery, so `50` in the skill with `50` Magery gives a quarter of it
- Let Poisoning coat all fencing weapons, arrows, and bolts, but no longer swords or knives:
    - Anyone can use poisoned weapons and ammunition, but every swing or shot risks poisoning the user, from `50%` at `0` Poisoning, to `5%` at `50`, and `0%` at `100`
    - Poisoned arrows and bolts are fired before clean ones, strongest poison first, and recovered ammunition is always clean
    - Poisoners with enough skill can see the strength of poison on weapons, arrows, and bolts by single-clicking them
- Adjust [Fletching](/fletching) to benefit archers in the field:
    - At `100` Fletching, ranged weapons attack `2` tiles farther
    - At `100` Fletching, the delay an archer must stand still to attack is reduced by half, from `1.0` to `0.5` seconds
    - At `100` Fletching, arrows and bolts that miss are twice as likely to drop, from `40%` to `80%`
- Adjust [Tracking](/tracking) to benefit archers in the field:
    - Ranged weapons gain a bonus to accuracy based on Tracking
    - Formula: `Hit Chance + (100% - Hit Chance) * Tracking / 200`
    - This effectively means that max Tracking adjusts current accuracy `50%` closer to a guaranteed hit
    - This bonus is doubled against fleeing enemies, meaning a grandmaster Tracker never misses a fleeing target
- Fix the [Lumberjacking](/lumberjacking) grandmaster bonus never applying, so axes now do `30%` bonus damage at `100` Lumberjacking instead of `20%`
- Prevent monsters from casting heals
- Prevent monsters from casting necro spells
- Edit treasure map description to make it T2A
- Reduce potion weight
- Make armor reduce damage by a percentage instead of a flat amount, so it protects against hard hits as well as light ones
- Make shields also reduce every hit by a small amount, on top of blocking
- Let swords critically strike for double damage, with a `10%` chance at `100` Swordsmanship

## 2026.11.19
- Add the Antimage rework, so characters with less Magery fight better:
    - Tactics adds up to `30` points of weapon skill when rolling to hit
    - Physical damage taken is reduced by up to `20%`
    - Hit points regenerate up to `5×` faster
    - All three bonuses are full at `0` Magery and shrink to nothing at `100`
    - Only players get the bonuses
- Strengthen the stealth archer ambush:
    - Raise the damage from each stealthed step to `0.1×`, for a total of `2.5×` after all `10` steps
    - Cap ambush damage against players at `2.0×`
- Fix [Young players](/young_player) being unable to Recall, Gate Travel, or use moongates
- Make wrestling moves automatic:
    - Armed players and human NPCs are disarmed, and everything else is stunned
    - Moves are only attempted when a punch hits, and need free hands
    - Moves no longer cost stamina
    - Any attempt starts a `10` second cooldown
    - The stun and disarm buttons now only explain that the moves are automatic
- Make Dexterity add `1.75` stones of carrying capacity per point, half as much as Strength
- Stop thrown weapons from being equipped
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
- Make attacking one's own [pet](/pet) non-criminal, so pets can be used to train weapon skills
- Show pets as allies to their owners
- Add more strongbox and trash barrel commands
- Fix the spyglass showing Trammel's moon phase
- Stop fighting one's own pets from blocking Recall and Gate Travel
- Make saying `claim` at a stable open the list of stabled pets
- Show the stealth archer's *You are in perfect position!* message only once

## 2026.11.17
- Add `Veterinary / 25` extra tiles to pet bandage range with [Veterinary](/veterinary)
- Halve bandage weight
- Raise runebook use range from `2` to `3`
- Lower runebook use cooldown from `7` seconds to `3`
- Remove non-T2A items from the Carpentry crafting menu
- Set house decay to `90` days
- Delete items in decayed houses instead of dropping them
- Make Meditation, potions, and Wrestling ignore equippable lights

## 2026.11.16
- Adjust nightmare spawn time to `1` to `2` hours
- Adjust silver steed spawn time to `0.5` to `1` hours

## 2026.11.15
- Fix monster-vs-monster damage (it was halved while adjusting monster-vs-player damage)
- Move the server's daily restart to a scheduled cron job
- Adjust various Lockpicking requirements
- Halve the weight of gold and reagents
- Show a custom description on marked recall runes
- Fix a bug with Magic Reflection sometimes failing
- Make potions stackable
- Split gold automatically when a stack reaches its maximum size
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
- Rebalance monster spellcasting: creatures with higher Magery now cast spells more often, and those with lower Magery cast less often

## 2026.11.12
- Add the [Shiny](/mount) mechanic to silver steeds and nightmares
- Revert the follower slot change (for example, dragons take `3` slots again)
- Block Recall, Mark, and Gate Travel to, from, and within the Lost Lands
- Remove fire steeds and acid elementals from spawners

## 2026.11.11
- Remove fire horn drop sources
- Refactor treasure map loot, and allow cascading
- Fix pets responding to partial custom names (for example, `a` no longer triggers `aa`)
- Disable Virtue Dungeon Armor rewards
- Disable seasonal events
- Reduce the blood elemental spawn count in Shame
- Fully disable the Bulk Order system
- Disable all quests except Grizelda's quest

## 2026.11.10
- Make all pets take up `1` follower slot (each character has `5` in total)

## 2026.11.09
- Fix pets given the `follow` command not ignoring enemies
- Set Peacemaking's cooldown to `10` seconds on success and `5` seconds on failure
- Restart the server automatically once a day at `12:00` GMT
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
- Let anyone use locked-down runebooks
- Add teleporters to reach Cyclops Valley from the south

## 2026.11.06
- Fix player corpses not turning to bones at `50%` of their duration
- Adjust player corpse decay to `60` minutes in total
- Monsters with Magery:
    - Now only cast Teleport when stuck
    - No longer cast Invisibility

## 2026.11.05b
- Fix the Cartography crafting menu:
    - Remove tattered wall maps and the wall map of Eodon
    - Move the star chart from last to first
- Allow smelting ore directly from a pack animal's inventory
- Fix pet follow speed to match player speed
- Remove crafting resource and special scroll drops from treasure maps
- Make fleeing monsters walk instead of run

## 2026.11.05a
- Fix random scroll drops all being low level
- Remove special resource drops from treasure maps
- Fix Magic Reflection, Reactive Armor, and Protection not stacking

## 2026.11.04
- Remove necromancer scroll drops from `15` additional monsters
- Disable random necromancer reagent drops from all monsters
- Change the `[Password` command to work without a GM present
- Allow Protection, Reactive Armor, and Magic Reflection to work at the same time
- Add the map level to the name of completed treasure maps

## 2026.11.03
These are the changes to ServUO's base, and the server's starting point.
- Set ServUO's era to T2A, which disables a lot of content not listed here
- Set the stat cap to `100`
- Disable champions
- Disable factions
- Enable duel arenas
- Enable guild PvP
- Set map geography to Felucca only
- Set map PvP and shove rules to Trammel
- Disable New Haven as a starting city
- Change moongates to Felucca only
- Disable creature bonding
- Change the swing cycle to be more like T2A
- Change the Provocation failure cooldown to `5` seconds
- Let Provocation target the bard who used it
- Change Moonglow Zoo spawns to avoid guard aggro
- Move the Council of Mages to its proper location
- Enable Recall to and from T2A
- Disable random necromancer scroll drops
- Disable necromancer scroll drops from imps (others exist)
- Stop instruments from dropping with modifiers
- Let boats be dry-docked by clicking the tillerman
- Tone down monster mage AI
- Stop mounts from tiring when damage is taken
- Change Magic Reflection to its old form
- Make followers move faster
- Give reagent vendors larger stocks
- Make mage vendors sell Recall and Mark scrolls
- Set boat decay to `1` day
- Set house decay to `7` years