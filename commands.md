---
title: Commands
description: Speech commands for NPCs, followers, and places, and the server commands players can use
published: true
date: 2026-11-19T07:49:07.476Z
tags: 
editor: markdown
dateCreated: 2026-11-19T00:06:15.205Z
---

# Commands
Commands are typed into the chat line. Most are phrases spoken to NPCs, followers, and objects, and a few are server commands that start with `[`.

## Speech Commands
Many actions on *Paradise* use speech: phrases said aloud to the right NPC, follower, or object. Commands for an NPC only work from nearby, and some need its name first, such as `Alice train`. Speech starting with an exclamation point and a space, like `! bank`, is converted into a yell, which carries farther than normal speech.

### Anywhere
| Phrase | Effect |
|:-|:-:|
| `guards` | Calls the town guards on nearby criminals, in a guarded town |
| `I must consider my sins` | Shows the character's murder counts |
| `I resign from my guild` | Leaves the character's player guild |
| `I renounce my young player status` | Gives up [Young](/young_player) status. |

### Bankers
| Phrase | Effect |
|:-|:-:|
| `bank` | Opens the bank box |
| `balance` | Shows how much gold is in the bank box |
| `withdraw <amount>` | Moves up to 5,000 gold from the bank box to the backpack |
| `check <amount>` | Writes a bank check for 5,000 to 1,000,000 gold |

### Vendors
| Phrase | Effect |
|:-|:-:|
| `vendor buy` | Opens the buy menu of nearby vendors |
| `vendor sell` | Opens the sell menu of nearby vendors |
| `<name> buy` | Opens one vendor's buy menu |
| `<name> sell` | Opens one vendor's sell menu |

### Other NPCs
| Phrase | Effect |
|:-|:-:|
| `<name> train` | Lists the skills a townsperson can teach, for a fee |
| `<name> time` | Asks a townsperson for the time |
| `<name> move` | Asks a townsperson to step aside |
| `join` | Joins the NPC guild of a nearby guildmaster |
| `resign` | Leaves the NPC guild of a nearby guildmaster |
| `disguise` | Buys a disguise kit from the Thieves' Guild guildmaster |
| `news` | Asks a town crier for the news |
| `appraise` | Asks a real estate broker to value a house deed |

### Places
Some places in the world respond to a spoken word.

| Phrase | Where | Effect |
|:-|:-:|:-:|
| `recdu` | Teleporter in Moonglow | Teleports to Papua, in the Lost Lands |
| `recsu` | Teleporter in Papua | Teleports to Moonglow |
| `doracron` | Serpent pillars in the seas of Britannia | Moves a boat and everyone on it to the Lost Lands sea |
| `sueacron` | Serpent pillars in the Lost Lands sea | Moves a boat and everyone on it back to Britannia |
| `cross` | Skara Brae's ferry points | Crosses the water between Skara Brae and the mainland |
| `om om om` | Shrine of Spirituality | Moves the speaker into the shrine |

The teleporters work within a few tiles. The serpent pillars only work from a boat within `10` tiles of the pillar, and the word must be said on its own from a [boat](/boat).

Escort quest commands, such as `destination`, are listed with the [quests](/world#quests).

Other speech commands are listed on their own pages:
- [Follower](/follower#commands) commands, such as `all follow me`
- [Stable](/stable) commands, such as `stable` and `claim`
- [House](/house) commands, such as `I wish to lock this down`
- Tillerman commands for boats, such as `forward` and `stop`

## Server Commands
Players can type commands in the chat line starting with `[` to check or change account and server details.

| Command | Effect |
|:-|:-:|
| `[Help` | Lists every command the player can use |
| `[HelpInfo` | Opens a window describing each command |
| `[Password <new> <new>` | Changes the account's password, typed twice to avoid mistakes |
| `[TimePlayed` | Shows how long the character has been played |
| `[Time` | Shows the current time |
| `[TimeStamp` | Shows the current date and time |
| `[WhatIsIt` | Targets an object and shows what type of object it is |

Guildmasters often ask for a certain amount of play time before accepting a new member, which `[TimePlayed` shows.