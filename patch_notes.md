---
title: Patch Notes
description: Every change to Paradise, newest first
published: true
date: 2026-11-28T14:59:01.887Z
tags: 
editor: markdown
dateCreated: 2026-11-04T19:38:55.944Z
---

# Patch Notes
Changes to *Paradise*, newest first.
## 2026.11.28
- Let [Carpentry](/carpentry) strengthen clubs, and [Blacksmithing](/blacksmithing) strengthen hammer picks, maces, mauls, and war maces, each by up to `15%` like staves
- Rework [Stealing](/stealing) to rob monsters and townsfolk:
    - Fill a creature's pocket on its first theft: once for monsters, and again after `2` to `6` hours for townsfolk
    - Fill pockets by the owner's work or Fame, and roll a lottery on each, from a gem pouch at `1` in `100` to a castle deed at `1` in `1,000,000`
    - Only allow pocket items to be stolen, never a monster's own loot or a vendor's stock, and delete pocket items when their owner dies
    - Stop Stealing from revealing the thief, and roll a `(10 + (100 - Stealing) / 2)%` chance to be caught on every attempt
    - Make caught monsters attack, and caught townsfolk shout *Thief!*, without flagging the thief a criminal
    - Require the Thieves' Guild to steal from townsfolk
    - Count lottery prizes as `1` stone when stolen
    - Remove the later-era special items stolen from monsters
- Make [Snooping](/snooping) spot lottery prizes on each theft, and let Thieves' Guild members peek into townsfolk's backpacks
- Let grandmasters of [Begging](/begging) pacify a monster fighting them for `30` seconds, with a `(Snooping + Stealing) / 200` chance and a `2` minute cooldown
- Add the Thief class to [stalkers](/stalkers#thief), and give the Pirate Remove Trap instead of Hiding
- Add the [jail](/jail) for thieves caught in guarded towns:
    - Sentence `1` minute, plus `1` for each offense on record, up to `60`, with one offense forgiven per day
    - Count sentences down only while online, and confiscate stolen items
    - Add cell locks that grandmaster lockpickers can pick, at `1` in `300` per attempt
- Add thieving rules to the [Karma towns](/stealing#karma-towns):
    - Require the town's Karma to steal there
    - Cost `1,000` Karma toward neutral when caught, instead of jail
    - Add town prizes at `1` in `250`: a silver weapon in Serpent's Hold and a level `5` treasure map in Buccaneer's Den
- Rework traps:
    - Stop [Telekinesis](/telekinesis) from setting off traps
    - Limit [Magic Untrap](/magic_untrap) to level `1` dungeon and treasure chests
    - Remove [Remove Trap](/remove_trap)'s Detecting Hidden requirement, and make its chance `(Remove Trap - Trap Power / 2) / 50`
- Make [guildmasters](/guilds) require `50` in their guild's skill instead of play time, and stop them counting join fees as donations
- Stop vendors from counting a single gold donation twice
- Only make a crook in the backpack [hum](/weapon_effects#shillelagh) after a bonk
- Add [vanishing](/stealth#vanish): using Stealth while visible with `100` Hiding and `100` Stealth hides a player at once, even in the middle of a fight, and starts Stealth's steps
    - Always succeeds, and counts as a Hiding-skill hide for ambushes
    - Needs armor below `26`, and doesn't work while mounted
    - Can't be used again for `2` minutes, with a message when it's ready
- Rework the [classes](/classes) into tanks, fighters, archers, stalkers, mages, tamers, bards, and crafters, with a page for each group
    - Add the Juggernaut, Grenadier, Puppetmaster, Wizard, Golemancer, Priest, Beastwarden, Packleader, and Skald classes
    - Rename Beastmaster to Whisperer
    - Give the Shepherd Cooking instead of Evaluating Intelligence, the Summoner Tailoring and Cooking instead of Anatomy and Evaluating Intelligence, and the Forager Cooking instead of Hiding
    - Move the Carpenter and the Paladin to tanks
    - Give the Blacksmith, Carpenter, and Beastwarden Alchemy instead of Healing, the Puppetmaster Cooking instead of Healing, the Monk Inscription instead of Tactics, and the Summoner Wrestling instead of Inscription
    - Rework the Hunter into a stealth sniper with Archery, Tactics, Anatomy, Poisoning, Tracking, Hiding, and Stealth
    - Rework the Paladin into a group healer, and give it and the Forager `65` Dexterity and `60` Intelligence
- [Cooking](/cooking):
    - Double the healing from eating to `Cooking / 10` per point of hunger filled
    - Make sweets restore mana instead of hit points
    - Add a `3` second wait between meals
    - Let alcohol lower hunger by `1`, at most once every `10` seconds and never to `5` or below
- Make heal potions heal up to four times their minimum and twice their maximum for [alchemists](/alchemy#healing), instead of adding `Alchemy / 10`
- Make players defend unarmed with [Wrestling](/wrestling#unarmed-defense) alone, instead of Anatomy and Evaluating Intelligence
- Make the [robe](/meditation#robes) bonus grow as mana drops, up to twice as fast when empty
- [Carpentry](/carpentry):
    - Let staves' Crushing Blows [flourish](/weapon_effects#crushing-blow) onto every monster around the wielder
    - Raise the wooden shield's Carpentry bonus to `25` armor, past every other shield
- Let [Discordance](/discordance#demibosses) work on demibosses, succeeding `Discordance / 200` of the time
- Change [Reactive Armor](/reactive_armor)'s maximum absorb to `(Magery + Meditation) / 4 + Inscription / 4`, so Inscription raises it from `50` to `75`
- Add a `10` second wait between lighting [explosion potions](/alchemy#explosion)
- Keep shields equipped while [casting](/magery#spells), so only weapons go to the backpack

## 2026.11.27
- Lower golem break down chance to `10%`
- Prune [Blacksmithing](/blacksmithing) to T2A:
    - Remove dragon scale armor and the metal keg
    - Fix the broadsword missing from the crafting menu
- Prune [Tailoring](/tailoring) to T2A:
    - Remove spined, horned, and barbed leather, the orc, bear, deer, tribal, and horned tribal masks, oil cloth, and the Krampus hat, boots, and talons
    - Remove bone armor and the orc helm from the crafting menu, so bone armor only drops as loot
    - Make carved corpses give only plain hides or leather, and no scales
    - Stop monsters from dropping bones, and stop bone piles and rib cages from being cut into bones
- Require enough [Magery](/magery) to have a chance of casting a spell before scribing it with [Inscription](/inscription)
- Make a failed craft lose half of each material instead of all of it
- Add [metal types](/armor#metal-types) to armor:
    - Make colored metal reduce spell damage instead of adding armor rating, up to `10%` for a full valorite set with a shield
    - Make `10%` of the ringmail, chainmail, plate, and shields dropped by monsters come in a colored metal
    - Let [Arms Lore](/arms_lore) judge how well armor's metal wards off magic
- Sell shovels at provisioners in every town
- Remove items from after T2A from vendors, such as skin tingeing tincture, interior decorators, commodity deeds, malleable alloy, solvent flasks, hoes, aquarium items, beeswax, plant bowls, crystals, and taxidermy kits
- Fix demibosses dropping two treasure maps
- Add charged [magic items](/magic_items):
    - Add magic jewelry and clothing with Agility, Bless, Cunning, Invisibility, Magic Reflection, Night Sight, Protection, Strength, or Teleport (rings only)
    - Add cursed jewelry with Clumsy, Curse, Feeblemind, or Weaken
    - Drop them unidentified, showing their effect and charges once identified
    - Drop them from the richest monsters, [treasure chests](/treasure_map), and [dungeon chests](/lockpicking#dungeon-chests), and `4` to `6` strong ones from every demiboss
    - Replace plain jewelry and clothing in dungeon chests with magic items
- Add [wands](/magic_items#wands) to monster loot, demibosses, treasure chests, and dungeon chests
- Fix level 3 and 4 dungeon chests never dropping their magic weapons and armor
- Make [Item Identification](/item_identification) succeed or fail in a single roll, and identify magic items too
- Let wands of identification identify magic items
- Show an item's name and properties on one line when single-clicked, instead of two

## 2026.11.26
- Refresh [Deceit](/deceit):
    - Rework spawns so each floor grows more dangerous, from skeletons and zombies on floor 1 to liches and lich lords on floor 4
    - Add `7` summoning braziers that call a random Deceit monster, with a `5` minute cooldown
    - Make summoned monsters vanish `1` hour after they are summoned
    - Give the levers on floor 2 and the switch over the floor 4 bone pit surprise effects
    - Remove the hidden teleporters from floor 4 to Despise and Fire
    - Add demiboss to floor 3
- Add the [Forgotten One](/forgotten_one), a demiboss locked away on floor 3 of Deceit:
    - Built for tanks, with `15,000` to `20,000` hit points, a fast poisoning melee attack, and low damage
    - Reached only through the pit on floor 4
    - Give every Deceit summoning brazier a `0.1%` chance to call him instead
    - Drops a large haul of gold and magic items, `500` potions, and a level `5` treasure map
- Add [spiteful memory](/forgotten_one#spiteful-memory), which drains a lich's or lich lord's mana on a weapon hit once every `5` minutes:
    - Dropped by the Forgotten One `10%` of the time
    - Crumbles if a lich or lich lord kills its owner
- Refresh [Covetous](/covetous):
    - Add skeletons to floor 1, replacing a few harpies and stone harpies
    - Add a switch puzzle to the floor 3 necropolis that reveals a piece of lore
- Add a door switch to each mage tower on floor 3 of [Shame](/shame)
- Lower the number of elementals on floor 2 of Shame
- Cap the shillelagh's bonk at `10×` damage and `20` mana
- [Shillelagh](/weapon_effects#shillelagh):
    - Scale bonk damage with [Magery](/magery), so a bonk reaches `10×` only at `100` Magery
    - Never let a bonk do less than `1×` damage
    - Restart the bonk cooldown on any hit with another weapon or bare hands
    - Train Mace Fighting on bonks instead of Herding
    - Only hum for players with a crook in hand or in their backpack
- Make magic and exceptional weapon damage flat, so critical strikes, ambushes, and bonks only multiply the weapon's own roll
- Make [silver](/magic_weapons#silver) weapons do double damage to the Lich King and the Forgotten One, like other undead
- Healing potions restore `Alchemy / 10` extra hit points for alchemists

## 2026.11.25
- Remove the pet and summon damage penalties against monsters, so all followers deal and take normal damage
- Make demibosses do double damage to hirelings, like pets and summons
- Shillelagh:
  - Add range to hit scaled with Herding
  - Make attack consume mana and scale damage based on mana consumed
  - Allow shillelagh to train Mace Fighting on guaranteed hits
  - Play sound/visual effects for shillelagh bonks
  - Allow meditation with a shepherd's crook
- Make [robes](/meditation#robes) shorten the delay between mana points outside a trance for tailors wearing no armor, by up to `25%` at `100` Tailoring
- Add [golems](/golem), invulnerable machines built with Tinkering and Inscription that fight nearby monsters for `30` seconds:
    - Add prototype, mechanical, and terror golems, needing `50`, `75`, and `100` Tinkering and Inscription and taking `1`, `2`, and `3` follower slots
    - Make each golem cost `3` gems and a Blade Spirits scroll, and drop back to the ground `50%` of the time
- Reorganize the [Tinkering](/tinkering) menu into new categories, and remove items from after T2A, such as bolas, faction traps, and theme pack lamps
- Make [hunger](/cooking#hunger) matter:
    - Stop hit point regeneration at hunger `5` or below
    - Drain `1` hit point per second at hunger `0`, down to `1`
    - Warn players when they get hungry, and every `60` seconds while starving
    - Spare Young players the penalties, but not the warnings
- Make eating heal `Cooking / 20` hit points per point of hunger filled, with no cooldown
- Remove items from after T2A from the [Cooking](/cooking) menu, such as wheat wort, tribal paint, and coffee

## 2026.11.24
- Rework the [classes](/classes), adding classes built around scaling skills, the shillelagh, and melee ambushes
    - Add the Armsmaster class, and move the Warrior to Fencing so it doesn't need Arms Lore
    - Rename Archer to Ranger
- Make [Arms Lore](/arms_lore) control most [weapon effects](/weapon_effects), from nothing at `0` to full strength at `100`:
    - Scale sword critical strikes with Arms Lore instead of Swordsmanship
    - Trigger Concussion Blow, Crushing Blow, and Paralyzing Blow with Arms Lore instead of Anatomy, on `25%` of hits at `100`
    - Scale the vigor sapped by one-handed maces with Arms Lore
    - Train Arms Lore on hits with weapons that have a weapon effect
    - Leave the shillelagh, crossbow volleys, wrestling stuns, poison, and ambushes unaffected by Arms Lore
- Concussion Blow:
    - Remove Concussion Blow from two-handed axes, so hits with axes and polearms no longer train Arms Lore
    - Make Concussion Blow a polearm-only [weapon effect](/weapon_effects#concussion-blow), triggered by [Anatomy](/anatomy) instead of Arms Lore, on `25%` of hits at `100`
- Rename the Shadow class to Hunter to differentiate it from Rogues
    - Lower spear damage to pay for Paralyzing Blow: short spears from `4` – `29` to `4` – `25`, and spears from `2` – `34` to `2` – `29`
    - Stop two-handed spears (pitchforks, short spears, and spears) from [ambushing](/ambush), since they're too long to strike with from hiding
    - Let daggers backstab: each stealthed step adds `0.35×` damage instead of `0.1×`, for `5×` after `10` steps
- Rename Smith to Blacksmith
    - Give two-handed maces a [Blacksmithing](/blacksmithing) splash: each Crushing Blow has a chance, up to `100%` at grandmaster, to hit every monster around the target for the same damage
    - Remove the Blacksmithing damage bonus from one-handed maces
    - Make the war axe a two-handed mace, with Crushing Blow and the splash
- Draw arrows and bolts from a fixed spot on the archer, raised while mounted, so every bolt of a crossbow volley starts where the archer stood when it fired
## 2026.11.23
- Rename the Sorcerer class to Summoner
- Refresh [Shame](/shame):
    - Add skeletons to represent dead miners
    - Add bone magi to represent dead mages
    - Increase monster count on floors 3 and 4
    - Fill dungeon out with spawners in empty areas
    - Remove non-T2A monsters
    - Add teleporters between towers on floor 3, islands on floor 4
    - Write lore and add context decorations (glyphs)
    - Add demiboss to floor 4
- Add the [Greater Elemental](/greater_elemental), a demiboss on floor 4 of Shame:
    - Built for a group, with `20,000` to `30,000` hit points and a weak attack
    - Teleports around the lagoon, summoning lesser elementals that give no loot or skill gains
    - Adds poison and blood elementals to its summons below half health
    - Drops a large haul of gold and magic items, `100` gems, `1,000` reagents, and a level `5` treasure map
- Add the [primal amulet](/greater_elemental#primal-amulet), which makes one elemental summon spell free every `10` seconds:
    - Dropped by the Greater Elemental `50%` of the time
- Rework [summons](/summon):
    - Make blade spirits, energy vortexes, and daemons take `4` follower slots
    - Make summoned animals and elementals take fewer follower slots as [Spirit Speak](/spirit_speak) rises, down to `1` each
    - Limit each character to one summoned elemental of each kind
    - Stop Summon Creature from conjuring a kind of animal the caster already has summoned
    - Make every summon spell never fail at `100` Spirit Speak
    - Make elementals in Shame drop summon scrolls, and daemons drop Summon Daemon scrolls
    - Show a summon's follower slot cost when there aren't enough free
- Add [scaling skills](/weapons#scaling-skills) that make weapons hit harder, for players only:
    - [Blacksmithing](/blacksmithing) adds up to `40%` damage to one-handed maces
    - [Carpentry](/carpentry) adds up to `15%` damage to black, gnarled, and quarter staves
    - [Mining](/mining) adds up to `100%` damage to the pickaxe, which no longer gets the [Lumberjacking](/lumberjacking) bonus
    - Each bonus builds to two thirds by `99.9`, with the last third at grandmaster, like Lumberjacking
    - Make the Lumberjacking bonus players only
    - Make the wooden shield gain up to `15` armor from its wearer's Carpentry, matching a heater shield at `100`
- Add the [shillelagh](/weapon_effects#shillelagh) weapon effect, which turns the shepherd's crook into a weapon for herders:
    - The first crook hit after a `9` second cooldown bonks for `1` to `10` times the crook's damage roll, rising with [Herding](/herding)
    - At `100` Herding, bonks never miss
    - Remove Crushing Blow from the shepherd's crook
- Rebalance [weapons](/dps):
    - Give the double axe, executioner's axe, two-handed axe, and large battle axe their own speed and damage
    - Make the cutlass slower and harder hitting, with a `17%` critical strike chance
    - Make the maul slower and harder hitting
    - Raise the pickaxe's damage
    - Double the damage of knives
- Make every [weapon effect](/weapon_effects) players only, so NPCs no longer land Concussion Blow or Paralyzing Blow
- Remove Disarm from [wrestling](/wrestling#wrestling-moves), so every move is a stun
- Let fencing weapons and knives [ambush](/ambush) from Hiding and Stealth, like bows and crossbows
- Fix ambushed monsters never becoming alert
- Change Liche's ring drop sources and rates, now a lottery drop from all liches

## 2026.11.22
- Rework [hirelings](/hireling):
    - Add the cleric, a cheap hireling who heals its employer, their pets and hirelings, and itself, limited to one per character
    - Place `2` hirelings in each tavern and `10` in the Jhelom fighting pit, with unhired hirelings replaced every hour
    - Make hirelings deal and take full damage against monsters, including demibosses
    - Make hirelings quit when their pay runs out, instead of vanishing with their gear
    - Give hirelings a horse while they follow their employer
    - Fix wages being `1` gold for anyone who paid before asking the price
    - Fix wages resetting, and pay draining twice as fast, after a restart
    - Fix unhired hirelings vanishing a few hours after a restart
    - Fix gold being lost when paying too little or paying a hireling that's already hired
- Give [Spirit Speak](/spirit_speak) power over a player's summons, scaling up to `100` Spirit Speak:
    - Summons last up to twice as long
    - Dispel and Mass Dispel are up to `75%` less likely to remove them, except when used by the summoner
    - Summoned air, earth, fire, and water elementals do up to `50%` more damage
    - At `100` Spirit Speak, the four elemental summon spells never fail
- Rebalance [pet](/pet#pets-in-combat) combat:
    - Pets' melee hits and spells do `25%` less damage to monsters
    - Monsters' melee hits and spells do `25%` more damage to pets
    - Demibosses' melee hits and spells do double damage to pets
    - A pet's melee hits on another player are halved, the same as a player's
    - A player's summoned creatures count as pets
- Strengthen the [Lich King](/lich_king):
    - Raise his hit points to `9,000` to `11,000`
    - Make him blink to a nearby spot every `5` to `10` seconds in combat, or back to his throne if he strays more than `12` tiles
    - Make his Animate Dead raise a bone knight beside him, with no corpse needed
    - Make him speak a phrase when casting each necromancy spell, even without a target
    - Fix Blood Oath never reflecting damage under T2A rules
    - Let demibosses path around obstacles
- Stop a second bandage on the same target from restarting one already in progress, so no time or bandages are lost (switching targets still cancels it)
- Adjust Cyclops Valley spawners to be more accurate to T2A
- Add titans, cyclopes, and wyverns to the Lost Lands desert
- Move the server to a new VPS

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
- Rename Antimage to [Valor](/valor), the warrior's virtue from Ultima lore
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