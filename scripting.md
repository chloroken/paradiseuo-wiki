---
title: Scripting
description: An overview of how to use TazUO's Legion scripting 
published: true
date: 2026-11-25T08:10:40.365Z
tags: 
editor: markdown
dateCreated: 2026-11-25T08:00:09.704Z
---

# Getting Started with TazUO Legion Macros

## What this guide covers

Legion scripts are plain Python files that drive the TazUO client through a global `API` object. This guide gets you from an empty file to five working macros: auto-bandage, skill trainer, corpse looter, attack-nearest and a heal-on-hotkey. Use it alongside the companion *TazUO Legion Python API Reference* for full method lists, and check exact signatures on the [official docs](https://tazuo.org/legion/legionapi/).

## Setting up

1. Open the Legion Scripting window from the TazUO menu. It lists every script in your `LegionScripts` folder inside the TazUO install directory.
2. Create a new `.py` file in that folder (or use the window's new-script option) and give it a clear name, such as `AutoBandage.py`.
3. Start the file with `import API`, then write your logic below it.
4. Click the script in the window to start or stop it. A running script shows as active; stopping it sets `API.StopRequested`.
5. Test with a one-liner first: `API.SysMsg("Hello from Legion")`. If the message appears in your journal, your setup works.

To bind a script to a key, either assign it in the client's hotkey options or register keys from inside a running script with `API.OnHotKey("F1", callback)` (shown in Example 5).

## Four patterns every macro uses

**The main loop.** Repeat until the user stops the script, and always pause so you don't flood the server.

```python
import API

while not API.StopRequested:
    API.ProcessCallbacks()   # lets hotkeys and timers fire
    # ... your logic ...
    API.Pause(0.5)
```

**Pauses.** `API.Pause(seconds)` takes seconds, not milliseconds. Most actions need 0.5–1 s between them; skills and bandages need longer.

**Targeting.** Trigger the action, wait for the cursor, then pick the target.

```python
API.CastSpell("Heal")
if API.WaitForTarget(timeout=3):
    API.TargetSelf()
```

**Journal checks.** Read server messages to react to failures. Passing `True` clears the matched line so it isn't seen twice.

```python
if API.InJournal("You must wait", True):
    API.Pause(2)
```

## Example macros

Each example is a complete script. Copy it into its own `.py` file and adjust the values marked in comments.

### 1. Auto-bandage below 80% health

```python
import API

THRESHOLD = 0.80   # heal when below 80% HP
DELAY = 8          # seconds to wait after a bandage; tune to your Dex/shard

while not API.StopRequested: # called to start listening for events
    p = API.Player
    if p.Hits < p.HitsMax * THRESHOLD:
        if API.BandageSelf():
            API.CreateCooldownBar(DELAY, "Bandage", 33)
            API.Pause(DELAY)
        else:
            API.SysMsg("Out of bandages!", 33)
            API.Pause(5)
    API.Pause(0.5)
```

### 2. Skill trainer

```python
import API

SKILL = "Hiding"   # any skill used with UseSkill
DELAY = 10.5       # skill cooldown in seconds

while not API.StopRequested:
    API.UseSkill(SKILL)
    API.Pause(DELAY)
    API.SysMsg(f"{SKILL}: {API.GetSkill(SKILL).Value}")
```

### 3. Loot gold from nearby corpses

```python
import API

GOLD = 0x0EED
looted = set()

while not API.StopRequested:
    corpse = API.NearestCorpse(2) # closest corpse within 2 tiles
    if corpse and corpse.Serial not in looted: # serial is the unique identifier
        API.UseObject(corpse.Serial)   # open it
        API.Pause(1)
        for item in API.FindTypeAll(GOLD, corpse.Serial):
            API.MoveItem(item.Serial, API.Backpack)
            API.Pause(0.8)
        looted.add(corpse.Serial)
    API.Pause(0.5)
```

### 4. Attack the nearest hostile

```python
import API

HOSTILE = [API.Notoriety.Gray, API.Notoriety.Criminal,
           API.Notoriety.Enemy, API.Notoriety.Murderer] # eligible targets array

while not API.StopRequested:
    target = API.NearestMobile(HOSTILE, 10)
    if target and not API.IsFriend(target.Serial):
        API.SetWarMode(True)
        API.Attack(target.Serial)
        API.HeadMsg("Target!", target.Serial, 33) # stsring, follow, hue
        API.Pause(2)
    API.Pause(0.5)
```

### 5. Heal yourself on a hotkey

```python
import API

def heal_self():
    API.CastSpell("Greater Heal")
    if API.WaitForTarget(timeout=3):
        API.TargetSelf()

API.OnHotKey("F2", heal_self)
API.SysMsg("Press F2 to heal")

while not API.StopRequested:
    API.ProcessCallbacks()   # required to read hotkeys
    API.Pause(0.1)
```

## Tips and troubleshooting

| Problem | Likely cause | Fix |
| --- | --- | --- |
| Script won't stop | Loop doesn't check `API.StopRequested` | Use `while not API.StopRequested:` |
| Hotkey does nothing | `ProcessCallbacks()` never runs | Call it in the main loop |
| "You must wait" spam | Actions sent too fast | Raise `API.Pause()` values |
| Wrong item found | Graphic ID differs on your shard | Check the item's graphic in-game and update the constant |
| Targeting misses | Cursor not up yet | Wait with `API.WaitForTarget()` before targeting |

- Start with long pauses and shorten them once the macro works. Many shards penalize or kick for action spam.
- Keep one job per script; run several scripts side by side and share state with `API.SetSharedVar`.
- Save settings that should survive restarts with `API.SavePersistentVar`.
- Check your shard's rules on unattended macroing before leaving a script running AFK.

Graphic IDs, hues and delays above are common defaults, so verify them on your shard. Full method signatures: [TazUO Legion API docs](https://tazuo.org/legion/legionapi/).