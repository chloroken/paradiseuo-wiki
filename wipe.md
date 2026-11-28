---
title: Wipe
description: A series of steps required to wipe the shard
published: true
date: 2026-11-28T16:05:40.262Z
tags: 
editor: markdown
dateCreated: 2026-11-28T16:05:40.262Z
---

# Beta Wipe Checklist

1. Rehearse the whole wipe on the local shard, using a copy of the live saves.
2. Check whether `Saves/Thievery` and `Saves/Customs` hold player data that should be cleared.
3. Pick a wipe time, announce it in UTC and Eastern, and add it to the patch notes.
4. Turn off the 11:59 UTC daily restart for wipe day.
5. Clear the help page queue.
6. Save the world, stop the service, and back up the whole `Saves` and `Backups` folders to a safe place.
7. Start the shard, keeping it closed to players.
8. Run the wipe script to delete houses, boats, followers (including stabled pets), player vendors, and player guilds.
9. Delete all player accounts, and decide what to do with owner account.
10. Clear any `Thievery` or `Customs` data, if step 2 found any.
11. Run `[XmlSpawnerRespawnAll`, and check for any old ServUO spawners or champion spawns it would miss.
12. Leave the server closed for a few hours so loose items decay and puzzle timers reset.
13. Walk the world to check towns, dungeons, puzzles, and containers that never decay.
14. Save the world and turn the daily restart back on.
15. Open the server and post the patch note.