---
title: Features
description: What Paradise is, its rules, and the major ways it differs from T2A
published: true
date: 2026-11-24T09:45:22.670Z
tags: 
editor: markdown
dateCreated: 2026-11-18T23:04:02.833Z
---

# Features
*Paradise* is an [Ultima Online](https://uo.com/) shard. It keeps the classic base design and old-school feel of [T2A](https://en.wikipedia.org/wiki/Ultima_Online:_The_Second_Age), adds clever reworks that open up more avenues of play, and makes quality-of-life changes where they help. It's intended for solo players and small groups, and PvP is consensual only.

The main design goals are:
- Build diversity, with weapon users just as valuable as mages, tamers, and bards
- Manually tuned spawns that stay true to T2A's monster placement and selection
- Custom quests and [demibosses](/demibosses) that don't wreck balance, drawn from real Ultima lore
- Reworks of stale systems, such as reputation, that deepen immersion
- A wiki that documents the shard's actual code, not just an interpretation of it

This page covers the shard's rules, then the significant ways that *Paradise* deliberately differs from its T2A base. Smaller tweaks are listed in the [patch notes](/patch_notes). Development is ongoing during alpha. See [Plans](/plans).

## Rules
### The Basics
- Players can't attack each other. Duel arenas and guild wars are the only PvP.
- Macroing is allowed, but macros that collect items or profit must be attended.
- New players are protected by the [Young player](/young_player) system.

### Accounts
- A maximum of `2` accounts are allowed per person.
- Each account can have `5` characters and `1` [house](/house).

### Decay
- Houses decay after `90` days without a refresh, and everything inside is destroyed.
- [Boats](/boat) sink `24` hours after their last refresh.

### Conduct
- There is zero tolerance for bigotry and disruptive behavior.
- PvM etiquette is enforced and bullying isn't tolerated.

## Fighter Rework
Characters who fight with weapons are enhanced to keep pace with mages, tamers, and bards in PvM.

- [Valor](/valor):
  - Characters who fight without magic are gripped by [the warrior's virtue](https://wiki.ultimacodex.com/wiki/Valor).
  - Valor grants fighting bonuses that diminish as Magery increases.
- [Armor](/armor#how-armor-works):
  - Armor damage reduction is percentage-based instead of flat, making it better against bigger hits.
  - Shields also reduce every hit, on top of blocking.
- [Wrestling Moves](/wrestling#wrestling-moves):
  - Wrestling's stun happens automatically, no button or macro needed.
  - Disarm is removed, so every move is a stun.
- [Poisoning](/poisoning):
  - Inflicting poison is now tied to Poisoning level, giving it a use in the field.
- [Ambush](/ambush):
  - Attacks with bows, crossbows, one-handed fencing weapons, and knives do bonus damage if they break Hiding.
  - Breaking Stealth further enhances the attack.
  - Daggers backstab for up to `5×` damage.
- [Weapon Identities](/weapon_effects):
  - Swords critically strike for double damage, and slower swords crit more often.
  - One-handed maces weaken a monster's blows by sapping its vigor.
  - Two-handed maces and staves can slow a monster's attacks.
  - Polearms halve a target's mana with Concussion Blow, aimed with Anatomy.
  - Herding turns the shepherd's crook into a shillelagh that bonks for up to `10` times damage.
  - Weapon effects are for players only.
  - [Arms Lore](/arms_lore) controls most weapon effects, so each fighter chooses whether to pay for them.
  - Weapon damage is rebalanced so more weapons are worth using.
- [Scaling Skills](/weapons#scaling-skills):
  - Lumberjacking, Carpentry, and Mining make their own weapons hit harder.
  - Blacksmithing lets two-handed maces splash Crushing Blows onto every monster around the target.
  - Carpentry makes the wooden shield as sturdy as a heater shield.
- [Carrying Capacity](/stats#carrying-capacity):
  - Dexterity adds carrying capacity, half as much per point as Strength.

## Archer Rework
Archers receive several enhancements that make ranged combat more effective.

- Valor, Poison, and Ambush:
  - Archers also benefit from Valor bonuses.
  - Arrows and bolts can be coated with poison.
  - Bows and crossbows can ambush from Hiding and Stealth.
- [Fletching](/fletching#fletching-and-archery):
  - Increases range, reduces time to shoot, and saves more arrows.
- [Crossbow Volley](/archery#crossbow-volley):
  - Crossbows fire up to `3` bolts per shot.
- [Tracking](/tracking#archery-accuracy):
  - Increases accuracy with ranged weapons.
  - At `100` Tracking, shots against fleeing targets never miss.

## Follower Enhancements
Controlling [followers](/follower) is a popular fantasy, so it's been enhanced in three major ways. Followers keep pace with their owner, even when the owner is mounted (hirelings will mount their own horse), and players can attack their own followers without becoming criminals to hone their skills. See [Training on Followers](/follower#training-on-followers).

### Tamers
Animal tamers get several changes that make training, healing, and keeping pets easier.

- During alpha, Animal Taming gains skill twice as fast as normal.
- A player's own pets appear green to them.
- Animal tamers can bandage pets from farther away as their Veterinary skill rises. See [Veterinary: Range](/veterinary#range).
- Saying `claim` to an animal trainer opens a list of stabled pets to choose from. See [Stable](/stable).
- Silver steeds and nightmares have a small chance to spawn Shiny, with a rare hue. See [Mount](/mount).

### Summoners
Mages who train [Spirit Speak](/spirit_speak) have enhanced summoning spells. See [Summon](/summon).

Spirit Speak:
- makes summons last longer.
- makes summons become more resistant to dispels.
- makes summoned air, earth, fire, and water elementals do more damage.
- makes summoned animals and elementals take fewer follower slots. See [Summon: Follower Slots](/summon#follower-slots).
- makes summon spells less likely to fail, never failing at `100` Spirit Speak

Related Changes:
- A player can have only one elemental of each kind at once.
- Elementals in Shame and daemons anywhere drop summon scrolls. See [Summon: Summon Scrolls](/summon#summon-scrolls).

### Hirelings
Paid followers found in taverns, cheap enough for any character. *Paradise* adds the Cleric hireling. See [Hireling](/hireling).

- Each tavern has `2` random hirelings and the Jhelom fighting pit has `10`.
- Unhired hirelings are replaced with new ones every hour.
- Hirelings deal and take full damage against monsters.
- Hirelings ride horses when commanded to follow.
- The cleric hireling heals its employer, their pets and hirelings, and itself, but has limited mana.

## Reputation
Fame gives a choice between better gem prices at high Fame and faster skill gain at low Fame, while Karma decides who can trade in Serpent's Hold and Buccaneer's Den. Templars and thugs outside those towns make Karma easy to raise or lower, and locked Karma is unlocked with shrine mantras. See [Reputation](/reputation).

## Other Changes
- Monsters hit players with attacks much harder than other shards.
- Pets and summons take double damage from demibosses. See [Follower: Followers in Combat](/follower#followers-in-combat).
- Starting items aren't protected, so they drop on death once a character is no longer Young. See [Young Player](/young_player#losing-young-status).