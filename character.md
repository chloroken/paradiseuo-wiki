---
title: Character
description: Classes, builds, and what makes a character
published: true
date: 2026-11-28T08:59:47.276Z
tags: 
editor: markdown
dateCreated: 2026-11-21T05:59:08.295Z
---

# Character
A character's build, or class, is determined by its stats, skills, and reputation.

## Building Blocks
- [Stats](/stats): Strength, Dexterity, and Intelligence, and what each one does.
- [Skills](/skills): every skill, including the ones that are disabled.
- [Reputation](/reputation): builds up passively while interacting with the world.

## Classes
Ultima Online doesn't have discrete classes. To play something like an evil warrior, one would spend stat points on Strength and Dexterity and skill points on weapon skills, then commit bad deeds to lower karma. The classes below are ideas, grouped by purpose.

## Tanks
Tanks are built to stand in front of a monster and outlast it. The Blacksmith, Carpenter, and Paladin weaken a monster's hits with [one-handed maces](/weapon_effects#sapping-vigor), while the Juggernaut simply heals through them.

| Class | Unique Qualities |
|:-|:-:|
| Blacksmith | Saps a monster's vigor behind a metal shield, then splashes Crushing Blows around its target |
| Carpenter | Blocks with the sturdiest shield, then flourishes a staff into every monster around it |
| Paladin | Saps vigor with a mace while casting Heal and Cure and keeping most of Valor |
| Juggernaut | Stacks food, potions, and bandages on top of Valor's toughness and regeneration |

### Blacksmith
The Blacksmith is a self-made tank. It forges its own weapons, armor, and shields at the anvil, and [repairs](/blacksmithing#repairing) them between fights, so it never depends on anyone else for gear. Its whole kit is metal, and that matters: plate and shields forged from [colored metal](/armor#metal-types) ward off spell damage, up to a tenth of it for a full valorite set with a shield. No other tank holds up as well against casters, such as liches and the Lich King.

In a fight, it holds the front with a one-handed mace and a metal shield. Every mace hit, powered by Arms Lore, saps the monster's vigor, so its melee hits land as if it were weaker. Shield blocks, Mace Fighting, and [Valor](/valor)'s accuracy and toughness keep the damage that does land low. When monsters bunch up, it switches to a war hammer or war axe. With Arms Lore behind it, a two-handed mace lands Crushing Blows that halve a monster's attack speed, and Blacksmithing makes each one [splash](/weapon_effects#crushing-blow) the same hit onto every monster around the target.

Its limits come from what it leaves out. Without Anatomy, it gets no Valor regeneration, and its bandages heal less and can't cure poison, so it carries cure potions. It has no ranged attack and no magic, so it walks everywhere and has to close the distance to anything it fights.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Blacksmithing, Mace Fighting, Tactics, Arms Lore, Parrying, Healing, and Resisting Spells
- Gear: one-handed mace, metal shield, and a war hammer or war axe, with colored metal plate
- Defense: Mace Fighting, shield blocks, Valor's accuracy and toughness, colored metal, and resisted spells
- Healing: bandages and potions
- Weakness: no Anatomy, so no Valor regeneration and bandages that can't cure poison

### Carpenter
The Carpenter is the woodworker's answer to the Blacksmith: a tank built around wood instead of metal. It crafts its own staves and wooden shields, and Carpentry makes a wooden shield the [sturdiest shield](/parrying#shields) in the game against weapons, with more armor than even a chaos shield. That makes it the best tank against monsters that hit hard in melee.

It tanks with a club and that wooden shield. A club is a one-handed mace, so with Arms Lore it saps a monster's vigor just like the Blacksmith's mace. When it's surrounded, it switches to a black, gnarled, or quarter staff, which Carpentry makes [hit harder](/weapons#scaling-skills). A staff's Crushing Blow slows its target, and Carpentry lets it flourish, sweeping the same hit through every monster standing next to the Carpenter. The Blacksmith's splash hits a cluster in front of it, but the Carpenter's flourish rewards being mobbed.

Wood can't be forged from colored metal, so its shield never wards off spells, and casters hurt it more than the Blacksmith. Like the Blacksmith, it has no Anatomy, so no Valor regeneration and no curing with bandages. A staff is two-handed, so flourishing means giving up the shield.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Carpentry, Mace Fighting, Tactics, Arms Lore, Parrying, Healing, and Resisting Spells
- Gear: club, wooden shield, and a black, gnarled, or quarter staff, with plate
- Defense: Mace Fighting, shield blocks, Valor's accuracy and toughness, and resisted spells
- Healing: bandages and potions
- Weakness: a wooden shield never wards off spells, and with no Anatomy its bandages can't cure poison

### Paladin
The Paladin is a holy knight: a mace-and-shield tank with just enough [Magery](/magery) to heal, cure, and bless itself. It weakens monsters' hits with a one-handed mace like the other tanks, and its `60` Anatomy lets its bandages cure poison. With only `40` Magery, it keeps most of Valor: three fifths of the accuracy and toughness a pure fighter gets, and some of the regeneration.

It fights in metal, so it can wear colored metal plate and a colored metal shield for protection from spells. In a fight it alternates between its mace and its spellbook. Heal and Cure keep it going between bandages, and spells like Bless and Protection prepare it before a pull. It's the most self-sufficient tank, and its utility spells make it useful in a group.

Its catch is timing. Casting a spell moves its mace and shield into the backpack, so every spell leaves it without its shield or Mace Fighting until it re-equips. Its low Magery limits it to the lower circles and weak damage spells. It also has less Dexterity, so its bandages are slower than a pure fighter's.

- Stats: `100` Strength, `40` Dexterity, `85` Intelligence
- Skills: Mace Fighting, Arms Lore, Healing, Parrying, Tactics, Resisting Spells, `40` Magery, and `60` Anatomy
- Gear: one-handed mace, shield, and spellbook, with plate
- Defense: Mace Fighting, shield blocks, most of Valor, colored metal, and resisted spells
- Healing: bandages and spells
- Weakness: casting moves its mace and shield to the backpack, so it must time its spells wisely

### Juggernaut
The Juggernaut is the immovable object. It gives up Tactics, and with it most of its damage, to stack three separate layers of healing on top of a shield, Valor's toughness, and Valor's five-fold regeneration. It isn't trying to kill quickly, only to still be standing when everything else has fallen.

Its healing layers each work on their own timer. Bandages heal steadily, and Anatomy lets them cure poison. Alchemy roughly doubles what a heal potion does for it, so a [potion](/alchemy#healing) gives a large, reliable heal every `10` seconds. Cooking turns [food](/cooking#eating-as-a-cook) into an emergency button: a few bites of savory food can restore its whole health bar in seconds. The price is hunger. Once its stomach is full, it has to wait for hunger to drop, or drink [alcohol](/cooking#alcohol) between fights, before it can eat for healing again.

It fights with a kryss or war fork and a shield, so it needs no Arms Lore, and wears plate, ideally colored metal. Without Tactics, it does about a third of the damage of other fighters and misses more often, so solo fights take a long time. It shines in groups, holding a demiboss while others do the damage.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Fencing, Anatomy, Parrying, Healing, Alchemy, Cooking, and Resisting Spells
- Gear: kryss or war fork and shield, with plate
- Defense: Fencing, shield blocks, Valor's toughness, and resisted spells
- Healing: food for bursts, potions in between, bandages for steady healing, and Valor's regeneration
- Weakness: no Tactics, so it does about a third of the damage of other fighters and misses more often

## Fighters
Fighters always take a weapon skill and Tactics, and most take Parrying and Anatomy for the rest of Valor.

| Class | Unique Qualities |
|:-|:-:|
| Armsmaster | Switches weapons to land sword, mace, and polearm effects on one target |
| Prospector | Fights with a pickaxe that hits twice as hard, and mines its own ore |
| Warrior | Gets full Valor with a sword and shield and a bow, without Arms Lore |
| Woodsman | Does the highest damage of any class, and chops wood |

### Armsmaster
The Armsmaster is a weapons expert who carries a small armory and always brings the right tool for the job. Arms Lore powers most [weapon effects](/weapon_effects), and Swordsmanship and Mace Fighting cover nearly every weapon that has one, so it can use whichever effect a fight calls for.

It opens with whatever fits the target. A sword lands [critical strikes](/weapon_effects#critical-strikes) that double its damage, a war hammer's Crushing Blow halves a monster's attack speed, a one-handed mace saps its vigor, and a polearm's Concussion Blow halves a caster's Intelligence, which needs Anatomy instead of Arms Lore. Since each effect lasts a while, it can land one, switch weapons, and stack another on the same target. Its Anatomy gives it Valor's regeneration and stronger bandages that cure poison.

It skips Parrying to fit both weapon skills, so it gets none of Valor's toughness and has no use for a shield. It takes the full weight of every hit, more than any other fighter, and juggling weapons takes attention and backpack space.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Swordsmanship, Mace Fighting, Arms Lore, Tactics, Anatomy, Healing, and Resisting Spells
- Gear: swords, polearms, maces, and war hammers, with plate
- Defense: its weapon skills, Valor's accuracy and regeneration, and resisted spells
- Healing: bandages
- Weakness: no Parrying, so it gets none of Valor's toughness

### Prospector
The Prospector is a miner who fights back. Mining doubles the damage of the pickaxe at grandmaster, turning a gathering tool into a weapon that keeps up with any sword. It fights with the same pickaxe it digs with, so it can head into a dungeon, clear a path, and mine the ore at the end of it without changing gear.

With a pickaxe in one hand and a shield in the other, it gets full Valor: accuracy, toughness, and regeneration. It's a sturdy, simple fighter that blocks, hits hard, and bandages itself, curing poison with its Anatomy. Mining also makes digging up [treasure](/treasure_map) easier, and its ore can go to a blacksmith for colored metal armor.

The pickaxe has no weapon effect, so the Prospector has no Crushing Blows, critical strikes, or other tricks. It's straightforward damage and nothing else, and like every fighter it travels on foot.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Mining, Swordsmanship, Tactics, Anatomy, Parrying, Healing, and Resisting Spells
- Gear: pickaxe and shield, with plate
- Defense: Swordsmanship, shield blocks, full Valor, and resisted spells
- Healing: bandages
- Weakness: the pickaxe has no weapon effect, so it has little utility

### Warrior
The Warrior is the most well-rounded fighter, and the easiest to play well. It has full Valor and needs no Arms Lore, because it uses weapons without weapon effects. A kryss or war fork with a shield are the strongest one-handed weapons that have no effect to pay for.

Up close, it fights sword and board: fast fencing hits, shield blocks, and every Valor bonus. When something stays out of reach, it switches to a bow, since Archery lets it fire from range with the same Tactics and Anatomy bonuses. Its bandages heal well and cure poison. It can handle almost anything reasonably well, without any one weakness for monsters to exploit.

What it trades for that reliability is anything special. It has no weapon effects, no magic, no crafting, and no way to control a fight, so it relies on doing steady damage and taking it well.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Fencing, Archery, Tactics, Anatomy, Parrying, Healing, and Resisting Spells
- Gear: kryss or war fork, shield, and bow, with plate
- Defense: Fencing, shield blocks, full Valor, and resisted spells
- Healing: bandages
- Weakness: no weapon effects and no utility

### Woodsman
The Woodsman is the hardest hitter in the game. Lumberjacking adds up to `30%` damage to axes, on top of Tactics, Strength, and Anatomy, and a two-handed axe's big hits make the most of it. It chops wood with the same axe, so it gathers lumber as easily as it fights.

It plays like a berserker: close the distance and swing as hard as possible. Axes have no weapon effect, so it needs no Arms Lore and spends the points on full Valor instead. Its hits with an axe also train Lumberjacking, so it grows into its damage just by fighting.

A two-handed axe leaves no hand for a shield, so it takes Parrying only for Valor's toughness and never blocks. It has no utility beyond damage, and plenty of hits get through, so it leans on bandages and regeneration between fights.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Lumberjacking, Swordsmanship, Tactics, Anatomy, Parrying, Healing, and Resisting Spells
- Gear: two-handed axes, with plate
- Defense: Swordsmanship, full Valor, and resisted spells
- Healing: bandages
- Weakness: no hands for a shield and no utility, so it only takes Parrying for Valor's toughness

## Archers
Archers fight from range with [Archery](/archery), keeping out of reach of what they shoot.

| Class | Unique Qualities |
|:-|:-:|
| Ranger | Never misses a fleeing target, and makes its own arrows |
| Grenadier | Bombs groups of monsters without Magery, and shoots poisoned bolts |

### Ranger
The Ranger is a wilderness archer and a hunter of anything that runs. [Tracking](/tracking) finds its quarry and makes its arrows more accurate, and at grandmaster its shots never miss a fleeing target. [Fletching](/fletching) lets it make its own bows, arrows, and bolts in the field, assuming there are birds around for feathers.

It fights at a distance and keeps it. Fletching also adds range, shortens the wait to shoot after moving, and recovers more of the arrows it fires, so it can reposition and keep shooting. A bow gives steady damage, and a crossbow fires volleys of several bolts at once. Its Tactics and Anatomy give it Valor's accuracy and regeneration, and its bandages cure poison.

Once something reaches it, the Ranger is in trouble. It has no shield, no Parrying, and no melee skill, and it wears studded leather to stay quick, so it has to keep moving.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Archery, Tactics, Anatomy, Tracking, Fletching, Healing, and Resisting Spells
- Gear: bows and crossbows, with studded leather
- Defense: range, Valor's accuracy and regeneration, and resisted spells
- Healing: bandages
- Weakness: weak once something reaches it

### Grenadier
The Grenadier is a back-line bomber and poisoner. It brews its own [explosion potions](/alchemy#explosion), poisons, and heal potions, then throws bombs into groups of monsters and shoots [poisoned](/poisoning) bolts at whatever's left. It's the only class that does real area damage at range without Magery.

Explosion potions can be thrown with a crossbow in hand, so it never has to switch weapons. Each bomb hits everything within `2` tiles, and its Alchemy adds damage to every one. Between throws, its crossbow bolts carry poison that Poisoning makes more likely to land. Alchemy also makes its heal potions far stronger, which stacks with its bandages.

Its power costs reagents, and a lot of them: every bomb, poison, and potion has to be brewed. Its explosions hit allies and pets as readily as monsters, so it has to place them carefully in a group, and a potion that goes off in its own backpack hurts it too. Like other archers, it struggles once something reaches it.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Alchemy, Archery, Tactics, Anatomy, Poisoning, Healing, and Resisting Spells
- Gear: crossbow and explosion potions, with studded leather
- Defense: range, Valor's accuracy and regeneration, and resisted spells
- Healing: bandages and stronger heal potions
- Weakness: goes through reagents fast, and its explosions hit allies too

## Stalkers
Stalkers use [Hiding](/hiding) and [Stealth](/stealth) to get into position, then strike before the enemy can answer. With `100` Hiding, all three can [vanish](/stealth#vanish) when a fight turns against them and walk away.

| Class | Unique Qualities |
|:-|:-:|
| Hunter | Ambushes from range with a crossbow, then pins the target with Paralyzing Blow |
| Rogue | Backstabs from stealth, then picks the chests its victims guarded |
| Puppetmaster | Sends golems in from hiding, then disarms and picks the chests |

### Hunter
The Hunter is a patient sniper. It stalks its prey unseen, lines up the shot, and opens with a heavy crossbow [ambush](/ambush). After ten stealthed steps, the ambush does two and a half times damage and can't miss, the biggest single hit of any weapon in the game.

Whatever survives the opening shot gets pinned. Its two-handed spear, poisoned with Poisoning, lands [Paralyzing Blows](/weapon_effects#paralyzing-blow) through Arms Lore that freeze the target in place, while poison ticks away at it. If the fight goes badly, it vanishes and resets.

A monster stays alert for a minute after an ambush, so the Hunter gets one big opener per target. Stealth limits it to leather, it has no Parrying or Anatomy, and it heals only with potions, so a long, straight fight wears it down quickly.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Fencing, Archery, Tactics, Arms Lore, Poisoning, Hiding, and Stealth
- Gear: heavy crossbow and two-handed spear, with leather
- Defense: stealth, vanishing, Valor's accuracy, and its weapon skills
- Healing: potions
- Weakness: stealth limits it to light armor, and it heals with potions only

### Rogue
The Rogue is a backstabber and a thief. It creeps up behind its target and opens with a poisoned dagger, where ten stealthed steps make the ambush do five times damage and never miss. Then it finishes the fight quickly with a kryss or war fork and picks the [dungeon chests](/lockpicking#dungeon-chests) its victims were guarding.

A Rogue's fights are short by design. The backstab does most of the work, poison keeps chipping away, and its Anatomy gives it Valor's regeneration between fights. Lockpicking turns every cleared room into loot, since dungeon chests hold gold, gems, magic items, and wands, and get richer the deeper they're found.

It's fragile once it has to stand and fight. Leather, no shield, no Parrying, and healing that comes only from potions mean a Rogue that loses the element of surprise should leave, which is what vanishing is for. Dungeon chests are also trapped, and without Remove Trap it has to take the hit or bring magic to disarm them.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Fencing, Tactics, Anatomy, Hiding, Stealth, Poisoning, and Lockpicking
- Gear: daggers, krysses, and war forks, with leather
- Defense: stealth, vanishing, Valor's accuracy and regeneration, and Fencing
- Healing: potions
- Weakness: fragile once it has to stand and fight, with no shield and potions only, so it leans on vanishing to escape

### Puppetmaster
The Puppetmaster is a dungeon lockpicker that never lifts a weapon. It builds [golems](/golem) with Tinkering and brings them to life with Inscription, sneaks up to a chest's guards, and lets its machines do the fighting. Once the room is clear, it disarms the chest's trap with Remove Trap, picks the lock, and takes the loot.

Its golems are invulnerable, attack the nearest monster on their own, and are ignored by monsters, so a hidden Puppetmaster is never in danger while they work. A terror golem lasts `30` seconds and can be unleashed again `30` seconds later, and it usually drops back to the ground to be picked up again. Its Healing patches up any mistakes, and it vanishes if something does spot it. That makes it a relaxed, low-stress way to delve dungeons, well suited to casual players.

Golems are weak next to a real fighter, and the Puppetmaster can't fight on its own at all. Each golem costs gems and a Blade Spirits scroll, which it has to buy since it has no Magery to scribe them, and now and then a golem breaks down for good. With no Anatomy, its bandages can't cure poison.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Tinkering, Inscription, Hiding, Stealth, Lockpicking, Remove Trap, and Healing
- Gear: golems, lockpicks, and Blade Spirits scrolls, with leather
- Defense: stealth, vanishing, and golems that do the fighting
- Healing: bandages
- Weakness: golems are weak and only last `30` seconds, and it can't fight on its own

## Mages
Mages always take Magery and Meditation. Mages who expect to be caught in melee defend with Wrestling or a weapon, while those who stay out of reach can take Tailoring and wear a [robe](/meditation#robes) for faster mana regeneration.

| Class | Unique Qualities |
|:-|:-:|
| Battlemage | Combines polearm hits and spells, and halves a caster's Intelligence |
| Monk | Stuns casters out of their spells with its fists |
| Shepherd | Bonks for up to ten times damage, then follows up with a spell |
| Summoner | Fields all four elementals at once |
| Wizard | Casts from a robe, fires wands between spells, and refills its mana with sweets |
| Golemancer | Builds its own golems and keeps one fighting almost nonstop |
| Priest | Heals a whole group with spells and bandages, and resurrects with bandages |

### Battlemage
The Battlemage is a classic T2A halberd mage. It combines the full spellbook with the slow, crushing hits of a polearm, landing a big swing and following it with a damage spell for burst damage few others can match. Its polearm's [Concussion Blows](/weapon_effects#concussion-blow), powered by Anatomy, halve a target's Intelligence, which devastates other casters.

Casting a spell unequips the polearm, but a polearm swings so slowly that there's plenty of time to cast between swings and pick it back up. Its full Magery gives it every utility and travel spell, and Evaluating Intelligence makes its damage spells hit hard.

With `100` Magery, it gets none of Valor's bonuses. It defends with Swordsmanship only while the polearm is in its hands, so it's defenseless every time it casts. It wears leather to keep its mana regeneration up, which leaves its body exposed.

- Stats: `100` Strength, `25` Dexterity, `100` Intelligence
- Skills: Swordsmanship, Tactics, Anatomy, Magery, Evaluating Intelligence, Meditation, and Resisting Spells
- Gear: polearm and spellbook, with leather
- Defense: Swordsmanship while holding its polearm and resisted spells
- Healing: spells
- Weakness: no defense while casting with its polearm put away

### Monk
The Monk fights with fists and magic, a martial artist with a full spellbook. It wears leather so its mana regeneration isn't slowed, and keeps its hands free for both punching and casting. Wrestling defends it whether it's punching or casting, so it's never caught without a defense.

Its signature is the [stun](/wrestling#wrestling-moves). Every punch that lands can try to freeze the target for `4` seconds, once every `10` seconds, succeeding half the time at grandmaster. A stunned caster can't start a spell, so the Monk shuts down enemy mages better than anyone, and frozen monsters give it time to cast.

Fists do little damage, so the Monk does most of its damage with spells, and it gets none of Valor's bonuses with `100` Magery. Leather is its only armor, so it relies on its spells, Wrestling, and stuns to stay safe.

- Stats: `100` Strength, `25` Dexterity, `100` Intelligence
- Skills: Magery, Evaluating Intelligence, Meditation, Wrestling, Anatomy, Tactics, and Resisting Spells
- Gear: fists and spellbook, with leather
- Defense: Wrestling and resisted spells
- Healing: spells
- Weakness: fists do little damage, and leather is its only armor

### Shepherd
The Shepherd is a spellcasting herder who turns a humble shepherd's crook into a weapon. Herding makes the crook a [shillelagh](/weapon_effects#shillelagh): every `7` seconds, its next hit spends mana to reach farther and bonks for up to ten times the crook's damage, growing with Herding and Magery. A bonk never misses.

It fights hit-and-run. It bonks, casts while the bonk recharges, and bonks again, and a bonk followed by a damage spell is a strong burst. Spells and re-equipping the crook don't restart the bonk's cooldown, so it can cast empty-handed and only pick up the crook to bonk. Bonks burn mana quickly, so Cooking lets it eat sweets to refill its mana in the middle of a fight.

It defends with Mace Fighting only while holding the crook, so it's completely vulnerable while casting. Without Evaluating Intelligence, its follow-up spells hit softer than a pure mage's, and it gets none of Valor's bonuses.

- Stats: `100` Strength, `25` Dexterity, `100` Intelligence
- Skills: Herding, Magery, Meditation, Tactics, Mace Fighting, Cooking, and Resisting Spells
- Gear: shepherd's crook and spellbook, with leather
- Defense: Mace Fighting while holding the crook and resisted spells
- Healing: spells, with sweets for mana
- Weakness: completely vulnerable while casting, and without Evaluating Intelligence its follow-up spells hit softer

### Summoner
The Summoner is a conjurer whose [summons](/summon) do the fighting. [Spirit Speak](/spirit_speak) makes its summons last up to twice as long, resist being dispelled, and take fewer follower slots, and it makes its elementals hit harder and its summon spells never fail at grandmaster. With enough Spirit Speak, it can field all four elementals at once.

It stays back while its summons hold the line. Inscription and Meditation make its Reactive Armor and Protection unusually strong, so whatever reaches it has a hard time hurting it or interrupting its spells. It wears a robe, which regenerates mana fastest when its mana is low, and eats sweets to refill mana after a round of summoning.

Its own damage spells are weak without Evaluating Intelligence, so it depends on its summons for damage. It has no melee defense of its own, and enemies that dispel its summons, or demibosses that do double damage to them, take away most of its strength.

- Stats: `100` Strength, `25` Dexterity, `100` Intelligence
- Skills: Magery, Meditation, Tailoring, Cooking, Inscription, Resisting Spells, and Spirit Speak
- Gear: spellbook, with a robe
- Defense: strengthened Reactive Armor and Protection, resisted spells, and its summons
- Healing: spells, with sweets for mana
- Weakness: no melee defense of its own, and its own damage spells are weak

### Wizard
The Wizard is a pure damage caster that never stops casting. Where other mages run dry and meditate, it keeps its mana up three ways: a robe that regenerates mana fastest when it's nearly empty, sweets that refill it in the middle of a fight, and [wands](/magic_items#wands) that cast without any mana at all.

It fights from range, casting damage spells powered by Evaluating Intelligence and firing a wand whenever it needs one more spell. Alchemy roughly doubles what its heal potions do, so it can heal without spending mana that should go to damage. In a long fight, it outlasts other casters.

It has no melee defense at all. No Wrestling, no weapon skill, and no armor mean anything that reaches it hits almost every time, so it has to keep its distance and kill quickly. Wands are found as loot and run out of charges, so it can't count on them forever.

- Stats: `100` Strength, `25` Dexterity, `100` Intelligence
- Skills: Magery, Meditation, Evaluating Intelligence, Tailoring, Alchemy, Cooking, and Resisting Spells
- Gear: spellbook and wands, with a robe
- Defense: range and resisted spells
- Healing: spells and stronger heal potions, with sweets for mana
- Weakness: no melee defense at all

### Golemancer
The Golemancer is a full mage who builds its own fighting machines. Tinkering builds its golems, and Inscription brings them to life, so it can make and use the strongest terror golems. Its Magery lets it scribe its own Blade Spirits scrolls for them, so it needs only gems to keep building.

It keeps a golem fighting almost nonstop, unleashing a new one as soon as the last winds down, and adds damage spells powered by Evaluating Intelligence on top. Monsters ignore golems, so they come for the Golemancer instead, and it has to hold them off itself. Inscription and Meditation make its Reactive Armor and Protection unusually strong for exactly that, and its robe keeps its mana flowing.

Every golem costs gems, and now and then one breaks down for good. With no Wrestling or weapon skill, it has no real melee defense beyond its spells, so it survives by keeping its protections up rather than by avoiding hits.

- Stats: `100` Strength, `25` Dexterity, `100` Intelligence
- Skills: Magery, Meditation, Evaluating Intelligence, Tailoring, Tinkering, Inscription, and Resisting Spells
- Gear: golems and spellbook, with a robe
- Defense: resisted spells and strengthened Reactive Armor and Protection
- Healing: spells
- Weakness: every golem costs gems, and monsters always come for the Golemancer

### Priest
The Priest is a group healer. It mends allies with Magery and bandages at the same time, cures poison with both, and brings fallen allies back with [bandage resurrection](/healing#resurrection), which its Healing and Anatomy make possible. A group with a Priest can push much deeper than one without.

It stays close to the group, healing whoever is hurt. Its robe regenerates mana fastest when it's low, which suits a healer that spends mana in bursts. Its Wrestling lets it hold off anything that reaches it while it keeps casting.

Without Evaluating Intelligence, its damage spells are weak, so it does little damage on its own and is slow to solo. It's built to keep others alive, not to kill.

- Stats: `100` Strength, `40` Dexterity, `85` Intelligence
- Skills: Magery, Meditation, Healing, Anatomy, Wrestling, Tailoring, and Resisting Spells
- Gear: spellbook and bandages, with a robe
- Defense: Wrestling and resisted spells
- Healing: spells and bandages
- Weakness: no Evaluating Intelligence, so its damage spells are weak

## Tamers
Tamers always take [Animal Taming](/animal_taming), Animal Lore, and Veterinary, and their [pets](/pet) do most of their fighting.

| Class | Unique Qualities |
|:-|:-:|
| Whisperer | Has pets and provoked monsters fighting for it at once |
| Druid | Moves a pet army with Gate Travel and heals pets from range |
| Beastwarden | Shoots from behind a pet that holds the monster's attention |
| Packleader | Fights beside its pet with a shield and full Valor |

### Whisperer
The Whisperer is a soft-spoken tamer that never swings a weapon, yet it's one of the strongest builds for hunting. It tames powerful pets and then uses its music to turn monsters on each other with [Provocation](/provocation), so its pets and the monsters it provokes are all fighting for it at once.

Its maximum Dexterity makes its pet bandages fast, and Veterinary lets it bandage from a distance. When a fight gets out of hand, [Peacemaking](/peacemaking) calms the monsters around it, and Hiding takes it out of sight.

It's exceptionally fragile. With no Valor, no armor skills, no Magery, and no weapon, anything that reaches it can hurt it badly, and it heals itself only with potions. Without Magery it can't Recall or Gate Travel, so moving its pets around is slow.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Animal Taming, Animal Lore, Veterinary, Musicianship, Peacemaking, Provocation, and Hiding
- Gear: instruments, with leather
- Defense: Hiding and Peacemaking
- Healing: potions
- Weakness: no true defenses, no Valor, and no Magery for travel, making it exceptionally fragile

### Druid
The Druid is a magical tamer and the most flexible of them all. It collects a pet army, moves it anywhere with Gate Travel, and keeps it alive with both magic and bandages. Greater Heal heals pets from range, bandages sped up by its `40` Dexterity heal them up close, and Cure and Invisibility can save a pet that's about to die.

It stays behind its pets and supports them, adding damage spells powered by Evaluating Intelligence. Its full Magery gives it every travel and utility spell, so it can reach any hunting ground quickly.

It has no melee defense of its own, so anything that gets past its pets is dangerous. Demibosses do double damage to every follower, so its pets need extra care in boss fights.

- Stats: `100` Strength, `40` Dexterity, `85` Intelligence
- Skills: Animal Taming, Animal Lore, Veterinary, Magery, Evaluating Intelligence, Meditation, and Resisting Spells
- Gear: spellbook, with leather
- Defense: its pets and resisted spells
- Healing: spells
- Weakness: no melee defense of its own

### Beastwarden
The Beastwarden is an archer with a bodyguard. Its pet charges in and holds the monster's attention while the Beastwarden shoots from behind it, and since the monster is busy with the pet, the Beastwarden can shoot freely.

It plays like a Ranger with a tank. Its Tactics and Anatomy give it Valor's accuracy and regeneration, and its bandages heal and cure itself while Veterinary keeps its pet going. It can still tame the strongest pets, since its Intelligence doesn't affect taming.

It has no Parrying, so no Valor toughness, and no Magery, so no Gate Travel to move its pets around. If its pet goes down, it's an archer with no melee skills and only studded leather between it and the monster.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Animal Taming, Animal Lore, Veterinary, Archery, Tactics, Anatomy, and Healing
- Gear: bows and crossbows, with studded leather
- Defense: its pet, range, and Valor's accuracy and regeneration
- Healing: bandages
- Weakness: no Parrying or Magery, so no Valor toughness and no Gate Travel for its pets

### Packleader
The Packleader fights side by side with its pet, behind a kryss and a shield. It's the only tamer that can take hits itself, with shield blocks and full Valor: accuracy, toughness, and regeneration.

Together, the Packleader and its pet split a monster's attention, and whichever one it isn't fighting does free damage. The pet adds its damage to the Packleader's steady fencing hits, and the Packleader can step in front to take a hit for a wounded pet while Veterinary patches it up.

It has no Healing for itself, so it relies on Valor's regeneration and potions, and no Resisting Spells, so casters hurt. Without Magery, it walks everywhere with its pet.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Animal Taming, Animal Lore, Veterinary, Fencing, Tactics, Anatomy, and Parrying
- Gear: kryss or war fork and shield, with plate
- Defense: Fencing, shield blocks, and full Valor
- Healing: Valor's regeneration and potions
- Weakness: no Healing for itself and no Resisting Spells, so casters hurt

## Bards
Bards always take [Musicianship](/musicianship), since every bard skill needs a good performance first.

| Class | Unique Qualities |
|:-|:-:|
| Minstrel | Uses all three bard skills to control a fight |
| Pirate | Runs treasure maps from start to finish on its own |
| Skald | Discords its target, then cuts it down with a two-handed axe |

### Minstrel
The Minstrel is a pure bard and the master of the battlefield. It provokes monsters into fighting each other, calms the ones it doesn't want to deal with, and weakens the rest with [Discordance](/discordance), then finishes them off with a bow or crossbow from afar.

Its music decides which fights happen. Provocation turns strong monsters into its weapons, Peacemaking stops anything that gets too close, and Discordance lowers a target's stats and skills by up to a fifth. Discordance even works on [demibosses](/demibosses), half the time at grandmaster, so the Minstrel has a role in every boss fight, weakening the boss while its Peacemaking and Provocation handle the boss's summons. Its Tactics gives its arrows Valor's accuracy.

Without Anatomy or Magery, its bandages can't cure poison, so it carries cure potions. It has no Parrying or melee skill, so it relies on its music to keep monsters away.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Musicianship, Peacemaking, Provocation, Discordance, Archery, Tactics, and Healing
- Gear: bows, crossbows, and instruments, with studded leather
- Defense: Peacemaking, range, and Valor's accuracy
- Healing: bandages and potions
- Weakness: without Anatomy or Magery it can't cure poison, so it carries cure potions

### Pirate
The Pirate is a treasure hunter who runs treasure maps from start to finish without help. It provokes monsters for map drops, decodes the maps with Cartography, Recalls or Gates to the dig site, and digs up the chest. Then it unlocks the chest with Lockpicking and disarms its trap with Magic Untrap, provokes the guardians that rise to defend it into fighting each other, and grabs the loot.

Its music and magic do all its fighting. Provocation turns the chest's guardians against one another, Hiding gets it out of trouble, and its full Magery gives it travel, utility, and healing spells.

It has almost no fighting ability of its own. With no weapon skill, no Wrestling, and no Valor, it depends on Provocation working, and a guardian that can't be provoked is a serious problem.

- Stats: `100` Strength, `25` Dexterity, `100` Intelligence
- Skills: Magery, Meditation, Musicianship, Provocation, Cartography, Lockpicking, and Hiding
- Gear: instruments and spellbook, with leather
- Defense: Hiding and Provocation
- Healing: spells
- Weakness: almost no fighting ability of its own

### Skald
The Skald is a war bard: a Viking-style warrior who sings its enemies weak, then cuts them down. It discords its target first, lowering its stats and skills, and then fights it with a two-handed axe and full Valor, so the weakened monster hits softer and is easier to hit.

Bard skills only need an instrument in the backpack, so it plays without putting its axe away. Axes have no weapon effect, so it needs no Arms Lore. Its Discordance works on demibosses too, half the time at grandmaster, which makes it a valuable fighter in boss fights. Its Anatomy gives it regeneration and bandages that cure poison.

It has no Resisting Spells and no Magery, so casters hurt and it walks everywhere. A two-handed axe means no shield, and half its attempts to discord a demiboss fail, so it doesn't always get its edge.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Musicianship, Discordance, Swordsmanship, Tactics, Anatomy, Parrying, and Healing
- Gear: two-handed axe and instrument, with plate
- Defense: Swordsmanship, full Valor, and a weakened target
- Healing: bandages
- Weakness: no Resisting Spells or Magery, so casters hurt, and half its attempts to discord a demiboss fail

## Crafters
Crafters make and gather what everyone else uses, and defend themselves with what they carry.

| Class | Unique Qualities |
|:-|:-:|
| Artisan | Crafts nearly everything: gear, potions, scrolls, and golems |
| Forager | Gathers ore, wood, and fish, and cooks its catch in the field |

### Artisan
The Artisan is the town's workshop in one character. It [crafts](/crafting) metal weapons and armor, wooden furniture and staves, clothing and leather armor, potions, scrolls, and tools, and Recalls between workshops to keep production moving. Nearly everything other classes use can come from an Artisan.

It isn't helpless outside town. With Tinkering and Inscription, it can build and unleash golems to defend itself, and its Magery gives it healing and utility spells. Its Alchemy roughly doubles what its own heal potions do, and its Tailoring lets it wear a robe for faster mana regeneration.

It has no weapon skill and no defensive skills, so it avoids real fights. Its value is in what it makes for others, not what it can kill.

- Stats: `100` Strength, `25` Dexterity, `100` Intelligence
- Skills: Alchemy, Blacksmithing, Carpentry, Inscription, Magery, Tailoring, and Tinkering
- Gear: crafting tools and golems, with a robe
- Defense: golems and spells
- Healing: spells and stronger heal potions
- Weakness: no weapon skill and no defensive skills

### Forager
The Forager gathers raw materials for everyone else. It mines ore, chops wood, and catches fish, then marks its own runes and Recalls home with the load.

It defends itself with the axe or pickaxe it already carries, which Lumberjacking and Mining make hit hard, using Swordsmanship and Tactics. When a fight goes badly, it cooks the fish it catches and eats them for burst healing, and its Magery adds healing spells.

It's a weak fighter, with no Anatomy, no Parrying, and `100` Magery that leaves it no Valor. It can't hide from what it can't beat, so it has to pick its gathering spots carefully.

- Stats: `100` Strength, `100` Dexterity, `25` Intelligence
- Skills: Mining, Lumberjacking, Fishing, Swordsmanship, Tactics, Magery, and Cooking
- Gear: axe or pickaxe, with leather
- Defense: Swordsmanship with its axe or pickaxe
- Healing: spells and food
- Weakness: a weak fighter that can't hide from what it can't beat