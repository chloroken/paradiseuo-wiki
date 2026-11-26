# Herding
Herding is the skill of guiding creatures with a shepherd's crook. It also turns the crook into a shillelagh, which bonks for up to `10` times damage.

## Herding Animals
Double-clicking a shepherd's crook and targeting a wild creature within `10` tiles, then a spot on the ground, tries to send them there. Only creatures that can be tamed can be herded, including monsters. A tamed creature *looks tame already* and can't be herded.

The chance depends on the animal's minimum taming skill. It rises evenly from `0%` at `30` below the minimum taming skill to certain success at `30` to `39` above it, so an animal that needs `50` to tame can't be herded below `20` Herding, and always moves at `90`. When the herder's skill is well above the animal's, the herder sees *That wasn't even challenging.*

On success, the herder sees *The animal walks where it was instructed to.* The animal walks straight toward the spot while it isn't fighting, and stops once it arrives or if it ends up more than `15` tiles away. A failure shows *You don't seem to be able to persuade that to move.*

## Shillelagh
In a player's hands, a shepherd's crook becomes a shillelagh. The first crook hit that lands after a `7` second cooldown is a bonk. It consumes `20%` of the attacker's current mana, up to `20`, and multiplies the crook's damage roll by `(Mana Consumed / 2) * (Herding / 100)`, up to `10×` with at least `100` mana and `100` Herding. At `100` Herding, a bonk never misses. Below that, a missed bonk isn't used up, so the next hit that lands bonks instead. See [Weapon Effects: Shillelagh](/weapon_effects#shillelagh).

The crook uses [Mace Fighting](/mace_fighting) to hit and defend. Herding adds no damage to the crook's other hits. At `100` Herding, a crook bonks about every third swing. With full mana for every bonk, it does about as much damage over time as a sword, but mana rarely refills that fast. See [Damage Per Second: Staves](/dps#staves).

A bonk that can't miss also skips that swing's chance to raise Mace Fighting.

The Shepherd class is built around the shillelagh. See [Character: Classes](/character#classes).

## Manual Training

| Herding | Creature | Location |
|:-|:-:|:-:|
| 0 – 30 | Sheep | Moonglow Zoo |
| 30 – 50 | Polar bear | Moonglow Zoo |
| 50 – 70 | Snow leopard | Moonglow Zoo |
| 70 – 90 | Bull | Moonglow Zoo |
| 90 – 100 | Giant frog | Moonglow Zoo |

## Macro Training
Before running the macro, the herder double-clicks the creature to train on so it becomes the `Last Target`. The macro then loops:
- `Use Item In Hand`
- `Wait For Target`
- `Last Target`
- `Wait For Target`
- `Last Target`
- `Delay 1000 ms`

This works because herding a creature to itself targets the ground under it. It takes `30` to `60` minutes to reach grandmaster from scratch.