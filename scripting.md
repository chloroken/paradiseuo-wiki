# Scripting
TazUO's [Legion scripting](https://tazuo.org/wiki/legion-scripting/) runs Python macros inside the client. Every command a script can use is listed in the [Legion API docs](https://tazuo.org/legion/legionapi/).

## Macro Structure
Most macros have the same three parts:

| Part | Description |
|:-|:-:|
| Import | Loads the tools a script needs, in this case `API` |
| Variables | Numbers that might be tweaked later, such as delays |
| Loop | The body of the macro, with its instructions and a delay |

This macro says *Hello, world!* every five seconds:

```
import API # load the tools

DELAY = 5.0 # a variable to tweak later

while not API.StopRequested: # loop until the macro is stopped
    API.Say("Hello, world!") # instructions
    API.Pause(DELAY) # delay
```

### Hotkeys and Callbacks
A macro can also define a function and bind it to a key, so the function runs each time the key is pressed. The loop listens for the key. Functions go after the variables and before the hotkey bindings and the loop.

This macro begs from the nearest innocent NPC within `5` tiles whenever `F1` is pressed:

```
import API

SKILL = "Begging"
MAXDIST = 5

def beg_npc(): # the callback function, run when F1 is pressed
    npc = API.NearestMobile([API.Notoriety.Innocent], MAXDIST)
    if not npc:
        return
    API.UseSkill(SKILL)
    if API.WaitForTarget(timeout=3):
        API.Target(npc)

API.OnHotKey("F1", beg_npc) # bind the key to the function

while not API.StopRequested:
    API.ProcessCallbacks() # reads hotkey input
    API.Pause(0.1) # always pause in a loop to avoid spamming commands
```

## Example Macros
These examples show common structures to copy and adapt.

### Auto-Bandage Below 80% Health
```
import API

THRESHOLD = 0.80   # heal when below 80% of maximum hit points
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
    API.Pause(0.5) # always pause in a loop to avoid spamming commands
```

### Skill Trainer
```
import API

SKILL = "Hiding"   # any skill used with UseSkill
DELAY = 10.5       # skill cooldown in seconds

while not API.StopRequested:
    API.UseSkill(SKILL)
    API.Pause(DELAY) # always pause in a loop to avoid spamming commands
    API.SysMsg(f"{SKILL}: {API.GetSkill(SKILL).Value}") # a formatted string
```

### Loot Gold From Nearby Corpses
```
import API

GOLD = 0x0EED # graphic ID, from Assistant -> Item Database -> Target Item Info
looted = set() # corpses already looted

while not API.StopRequested:
    corpse = API.NearestCorpse(2) # closest corpse within 2 tiles
    if corpse and corpse.Serial not in looted: # the serial identifies the corpse
        API.UseObject(corpse.Serial) # open the corpse
        API.Pause(1)
        for item in API.FindTypeAll(GOLD, corpse.Serial): # every gold pile inside
            API.MoveItem(item.Serial, API.Backpack) # drag it to the backpack
            API.Pause(0.8)
        looted.add(corpse.Serial)
    API.Pause(0.5) # always pause in a loop to avoid spamming commands
```

### Attack the Nearest Hostile
```
import API

HOSTILE = [API.Notoriety.Gray, API.Notoriety.Criminal,
           API.Notoriety.Enemy, API.Notoriety.Murderer] # eligible targets

while not API.StopRequested:
    target = API.NearestMobile(HOSTILE, 10)
    if target and not API.IsFriend(target.Serial):
        API.SetWarMode(True)
        API.Attack(target.Serial)
        API.HeadMsg("Target!", target.Serial, 33) # text, who it follows, hue
        API.Pause(2)
    API.Pause(0.5) # always pause in a loop to avoid spamming commands
```

### Self-Heal on a Hotkey
```
import API

def heal_self(): # callback function
    API.CastSpell("Greater Heal")
    if API.WaitForTarget(timeout=3):
        API.TargetSelf()

API.OnHotKey("F2", heal_self) # hotkey
API.SysMsg("Press F2 to heal") # journal message

while not API.StopRequested:
    API.ProcessCallbacks() # required to read hotkeys
    API.Pause(0.1) # always pause in a loop to avoid spamming commands
```
