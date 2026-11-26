# Follower
A follower is a creature that follows a character and fights for them. There are three kinds: [pets](/pet) are tamed, [hirelings](/hireling) are paid, and [summons](/summon) are conjured with Magery. [Mounts](/mount) are pets too. Most rules here apply to every follower, and the tables below show where the kinds differ.

| Rule | Pets | Summons | Hirelings |
|:-|:-:|:-:|:-:|
| Take follower slots | Yes | Yes | Yes |
| Can fail to obey | Yes | No | No |
| Loyalty and feeding | Yes | No | Yes |
| Pack Instinct | Yes | Yes | No |
| Can be stabled | Yes | No | No |

## Follower Slots
Each character has `5` follower slots. A character can't take on a follower that needs more slots than they have free.

| Follower | Slots |
|:-|:-:|
| Most pets, such as horses and bears | 1 |
| Strong pets, such as drakes | 2 |
| The most powerful pets, such as dragons | 3 |
| Hireling | 2 |
| Blade spirit, energy vortex, or daemon | 4 |
| Summon Creature's animal | 1 – 2 |
| Air, earth, fire, or water elemental | 1 – 4 |

Summoned animals and elementals take fewer slots as their caster's Spirit Speak rises. See [Summon: Follower Slots](/summon#follower-slots). See [Pet: Notable Pets](/pet#notable-pets) for the slots of individual pets.

## Commands
Followers are commanded by speech, with phrases like `all follow me`, `all guard me`, and `dragon kill`. See [Commands](/commands).

Pets don't always obey, depending on their owner's skills and their Loyalty. See [Pet: Obeying Commands](/pet#obeying-commands). Hirelings and summons always obey. Blade spirits and energy vortexes can't be commanded at all, and fight on their own.

A follower told to follow runs to catch up when it's more than `5` tiles behind, and paths around obstacles to reach its owner, unlike wild monsters. Followers keep pace with their owner, even when the owner is mounted.

Followers can follow their owner into houses. Untamed creatures can't enter houses.

## Followers in Combat
Followers deal and take normal damage against monsters. Demibosses are the exception: their melee hits and most of their spells do double damage to every follower, whether pet, hireling, or summon.

This applies to melee hits and spells. Breath, poison, and Fire Field do their normal damage. A follower's melee hits on another player are halved, the same as a player's. See [Combat: Damage](/combat#damage).

[Spirit Speak](/spirit_speak) strengthens a player's summons, and summoned elementals do up to `50%` more damage.

## Training on Followers
Players can attack their own followers to train combat skills, and heal their pets to train [Veterinary](/veterinary).
- Attacking one's own follower is never a criminal act.
- Followers don't fight back when their owner attacks them.
- A player's own pets appear green to them.
- Players and their pets can't attack other players' pets.

## Loyalty
Every pet and hireling has a hidden Loyalty value from `0` to `100`. Summons have none. A newly tamed pet starts at `100`, and Animal Lore shows how happy a pet is.

Once an hour, every pet and hireling in the world loses `10` Loyalty. Stabled pets and pets being ridden don't lose Loyalty. A pet that reaches `0` *looks around desperately*, then decides it is better off without a master and goes wild. A hireling at `0` walks off, even if its pay hasn't run out. See [Hireling: Loyalty](/hireling#loyalty).

An unfed pet or hireling at full Loyalty leaves after about `10` hours.

## Feeding
Pets and hirelings are fed by dropping food on them. Only their favorite food works. Animal Lore reveals a pet's favorite food, and hirelings eat meat. Each piece of food in the stack has a `50%` chance to add `10` Loyalty, up to the maximum of `100`. If any of it worked, the follower *looks happier*.

Feeding a stack is more reliable than feeding one piece, and a stack of `20` almost always fills a follower back to full. A follower eats the whole stack even after its Loyalty is full, so extra food is wasted.

Food also restores `15 * Pieces - 50` stamina, so a stack of `4` or more is needed to restore any.

## Death
**Pet and hireling death is permanent. GMs cannot resurrect them.** A summon vanishes when it dies or its time runs out. See [Summon](/summon).