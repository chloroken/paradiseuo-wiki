---
title: Scripting
description: An overview of how to use TazUO's Legion scripting 
published: true
date: 2026-11-25T08:48:21.348Z
tags: 
editor: markdown
dateCreated: 2026-11-25T08:00:09.704Z
---

# Getting Started with TazUO Legion Scripting
Making a [Legion Script](/https://tazuo.org/wiki/legion-scripting/) macro with TazUO is easier than it looks. See: [TazUO Legion API docs](https://tazuo.org/legion/legionapi/).

## Macro Structure

Most macros use the same structure:

| Section | Description |
|:-|:-:|
| Import | This section "imports" the proper tools, in this case "API" |
| Variables | Numbers that might be tweaked later, like delays |
| Loop | The guts of the macro, contains instructions and a delay |

So putting it together, let's make a macro that says "Hello, world!" every five seconds:

```python
import API # import the proper tools

DELAY = 5.0 # the variable delay to control later

while not API.StopRequested: # the loop, it goes until a "stop" is "requested"
    API.Say("Hello, world!") # instructions
    API.Pause(DELAY) # delay
```

A fourth structure of macros is hotkeys and callback functions. A function can be defined in a macro and called by that macro as many times as it wants, executing its instructions repeatedly. To bind a callback function to a key, the loop can be used to listen for that key. Callback functions should be inserted after defining variables, but before the hotkey bindings and the loop. Putting this into practice, here is a macro that continually begs the closest innocent NPC within 5 tiles.

```python
import API

SKILL = "Begging" # set up some variables
MAXDIST = 5

def beg_npc(): # this is the callback function, we will "call" it from the loops
		npc = API.NearestMobile([API.Notoriety.Innocent], MAXDIST)
    API.UseSkill(SKILL)
    if API.WaitForTarget(timeout=3):
        API.NearestEntity()

API.OnHotKey("F1", beg_npc) # here is the hotkey and callback function it calls

while not API.StopRequested:
    API.ProcessCallbacks() # this reads hotkey input
    API.Pause(0.1) # always use a delay in loops to prevent call spam
```

## Example Macros
But scripting has so much more potential. Here are five examples lay out various structures to copy.

### 1. Auto-bandage below 80% health

```python
import API

THRESHOLD = 0.80   # heal when below 80% HP
DELAY = 8          # seconds to wait after a bandage

while not API.StopRequested:
    p = API.Player
    if p.Hits < p.HitsMax * THRESHOLD:
        if API.BandageSelf():
            API.CreateCooldownBar(DELAY, "Bandage", 33)
            API.Pause(DELAY)
        else:
            API.SysMsg("Out of bandages!", 33)
            API.Pause(5)
    API.Pause(0.5) # always use a delay in loops to prevent call spam
```

### 2. Skill trainer

```python
import API

SKILL = "Hiding"   # any skill used with UseSkill
DELAY = 10.5       # skill cooldown in seconds

while not API.StopRequested:
    API.UseSkill(SKILL)
    API.Pause(DELAY) # always use a delay in loops to prevent call spam
    API.SysMsg(f"{SKILL}: {API.GetSkill(SKILL).Value}") # a formatted string
```

### 3. Loot gold from nearby corpses

```python
import API

GOLD = 0x0EED # graphic ID, can get from Assistant -> Item Database -> Target Item Info
looted = set() # a structure to keep track of which corpses have been looted

while not API.StopRequested:
    corpse = API.NearestCorpse(2) # closest corpse within 2 tiles
    if corpse and corpse.Serial not in looted: # serial is the unique identifier
        API.UseObject(corpse.Serial)   # open it corpse by identifier
        API.Pause(1)
        for item in API.FindTypeAll(GOLD, corpse.Serial): # loop through items
            API.MoveItem(item.Serial, API.Backpack) # drag drop items
            API.Pause(0.8)
        looted.add(corpse.Serial)
    API.Pause(0.5) # always use a delay in loops to prevent call spam
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
    API.Pause(0.5) # always use a delay in loops to prevent call spam
```

### 5. Heal yourself on a hotkey

```python
import API

def heal_self(): # callback function
    API.CastSpell("Greater Heal") # instructions
    if API.WaitForTarget(timeout=3):
        API.TargetSelf()

API.OnHotKey("F2", heal_self) # hotkey
API.SysMsg("Press F2 to heal") # journal output

while not API.StopRequested: # loop
    API.ProcessCallbacks()   # required to read hotkeys
    API.Pause(0.1) # always use a delay in loops to prevent call spam
```