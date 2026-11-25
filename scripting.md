---
title: Scripting
description: An overview of how to use TazUO's Legion scripting 
published: true
date: 2026-11-25T08:14:49.827Z
tags: 
editor: markdown
dateCreated: 2026-11-25T08:00:09.704Z
---

# Getting Started with TazUO Legion Macros

## Example macros
Making a [Legion Script](/https://tazuo.org/wiki/legion-scripting/) macro with TazUO is easier than it looks. These five examples lay out various structures to copy.

### 1. Auto-bandage below 80% health

```python
import API

THRESHOLD = 0.80   # heal when below 80% HP
DELAY = 8          # seconds to wait after a bandage; tune to your Dex/shard

while not API.StopRequested: # called to start listening for events
    p = API.Player
    if p.Hits < p.HitsMax * THRESHOLD: # algebraic conditional
        if API.BandageSelf():
            API.CreateCooldownBar(DELAY, "Bandage", 33)
            API.Pause(DELAY)
        else:
            API.SysMsg("Out of bandages!", 33)
            API.Pause(5)
    API.Pause(0.5) # always use a delay to prevent call spam
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
        API.UseObject(corpse.Serial)   # open it corpse by identifier
        API.Pause(1)
        for item in API.FindTypeAll(GOLD, corpse.Serial): # loop through items
            API.MoveItem(item.Serial, API.Backpack)
            API.Pause(0.8)
        looted.add(corpse.Serial)
    API.Pause(0.5) # always use a delay to prevent call spam
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
    API.Pause(0.5) # always use a delay to prevent call spam
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
    API.Pause(0.1) # always use a delay to prevent call spam
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