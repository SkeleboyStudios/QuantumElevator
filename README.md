# QuantumElevator
Quantum Elevator is a Roblox game where you test out weapons to blow up baddies, collect nanite and then
use the nanite to get even better weapons! Level up, improve stats, get armor, and see how deep into
the Quantum Elevators you can go!

This is essentially the design document and issue tracker for implementing the ideas here into the game itself.

The game itself can be found [here](https://www.roblox.com/games/14807778375/Quantum-Elevator) and any questions
can be answered on the skeleboy studios discord channel [here](https://discord.com/channels/915313727841108029/1153017030052696175)

# Gameplay

Click-to-move where the player selects from 6 different weapons, each one tied to a key or mouse click.
Also 'I' opens the inventory and 'P' your skill points.

![keyboard layout](/assets/skills-and-keys.png "default keyboard layout")

## Game Loop

Buy cool weapons from the stockroom, which is in the lobby but can appear either inside an elevator with cheaper
prices and sometimes exclusive gear. Take the weapons into the elevator to fight baddies, collect research experience
to make your way up the echeleons of academia, and get nanite to improve and get new weapons and armor. See what level
elevator you can make it to.

## Equipment

Equipment will determine gameplay for the most part. How your character moves, dodges, attacks will all be determined
by what equipment your character is using.

### Cores

Cores determine basic style of gameplay. It determines how your energy is collected, used, regenerated, and what weapons
can be equipped. There are several to choose from. Each one besides Solar Powered is unlockable via game pass.

#### Solar Powered

The default core. Has a maximum energy capacity and regenerates over time.

#### Kinetic

The one-two punch kind of core. Use some attacks to GENERATE energy and use the stored energy for big payoffs!

#### Docking Bay

The docking system allows you to have automated drones and turrets attack nearby enemies, dock to rechage and switch out,
and attack again! Choose from many different drones with different effects and abilities!

#### Combo System

Hit enemies with smaller attacks to build up combo points, and unleash them in devastating finshing moves. Can be physical
melee abilities, but also a ranged variation that throws flasks to deal elemental damage and cause effects like slow and
poision.

### Weapons

Weapons are the key skills used in the game. You can equip up to 5 (6 with a gamepass!) that can give you all kinds of
abilities from teleporting across the room to summoning meteors from the sky! Each weapon will have a range of power in
the ability, so to get the *perfect* weapon you may have to get the right one several times! The weapons are also tied to
their core, so without the right core you can't equip the weapon.

|    Name    |   Core  |                                               Ability                                      |
| ---------- | ------- | ------------------------------------------------------------------------------------------ |
| Laser Gun  |  Solar  | For [10-25] energy shoots [3-50] beams in a spread pattern dealing weak physical damage.   |
| Flame Thrower    |  Solar  | For [5-20] energy per second spread out flames in front of you dealing weak fire damage and causing burning near impact for [25-75]% fire damage for [3-10] seconds.               |
| Ice Dart   |  Solar  | For [10-20] energy shoots [1-25] darts of ice out in a circular pattern dealing weak frost damage and has adds [1-2] stacks of chill that can freeze for up to [1.5-2.25] seconds     |
| Concussive Blast     |  Solar  | For [35-55] energy shoots a blast of air outward deflecting any projectiles and dealing medium cold damage and adds [3-5] stacks of chill that can freeze for up to [2-3] seconds|
| Ice Armor  |  Solar Kinetic Dock Combo | Generates a shield around you for 3 minutes that grants a medium amount of armor and adds [2-5] stacks of chill that can freeze for up to [0.5-1.5] seconds                          |
| Plasma Armor      |  Solar  Kinetic Dock Combo | Generates a shield around you for 3 minutes that grants a lot of armor and thorns.         |
| Energy  Armor      |  Solar Kinetic | A percentage of your health is converted to a percentage of your energy instead.           |
| Teleport |  Solar Kinetic Dock Combo | Teleport to the cursor, up to [25-50] yards. [2.5-15] second cooldown. |
| Poison Gas |  Solar  | For [30-50] energy shoots out a canister of poison gas. Enemies in the gas clouds take medium poison damage.   | 
| Ice Storm  |  Solar Kinetic  | For [45-90] energy create a blizzard at target location, pelting down ice shards that deal high ice damage and adds [4-8] stacks of chill that can freeze for up to [2-3] seconds to all enemies in the area   |
| Meteor     |  Solar Kinetic | For [55-90] energy summon a meteor to drop in target area after [0.75-2.25] seconds that deal massive fire damage to anything in the area, but also burns for [110-225]% fire damage to enemies in the flames that last [5-15] seconds       |
| Levitation | Solar Kinetic Dock Combo | Causes the user to levitate and not be affected by terrain and ground effects like lava or fire. Lasts [3-10] seconds and has a [300-600] second cooldown. |
| Hurricaine | Solar Kinetic | For [90-150] energy summon a storm that follows you around dealing medium physical damage to enemies in the area. |
| Thunder Hammer | Kinetic | Generates [30-50] energy per hit, dealing medium lightning damage to enemies hit and kocking them back. |
| FIre Hammer | Kinetic | Generates [20-45] energy per hit, dealing medium fire damage and igniting the area for [15-20]% fire damage. |
| Ice Hammer | Kinetic | Generates [15-40] energy per hit, dealing medium ice damage and adding [3-8] stacks of chill that can freeze for up to [1.5-3] seconds. |
| Taunt | Kinetic | Generates 100 energy but causes all nearby enemies to focus their attacks on you. [15-45] second cooldown. |
| Defensive Array | Kinetic Dock | For [35-45] energy summons a defensive array at your location. Friendly units in the array take [25-50]% less damage. |
| Offensive Array | Kinetic Dock | For [35-45] energy summons an offensive array at your location. Friendly units in the array deal [55-85]% more damage. |
| Fire Walk | Solar Kinetic | For [75-125] energy, leave a trail of fire where you walk for the next [10-35] seconds. |
| Frost Nova | Solar Kinetic | For [55-90] energy, blast out a nova of frost dealing light ice damage and adding [6-10] stacks of chill that can freeze for up to [1.5-3] seconds. |
| Whirlwind | Kinetic | For [10-25] energy per second, summon swirling lazer blades that fly around you dealing heavy physical damage to nearby enemies. Also pulls in nearby enemies to slice them better! |
| Trample | Kinetic | For [45-70] energy trample through an area causing a patch of the ground that deals heavy physical damage to any enemy in it. |
| Charge | Kinetic | Generates [50-75] energy while charging at and dealing medium physical damage to the target. Has a [15-45] second cooldown. |


### Armor

### Jewels

### Runes

### Charms

## Chests

### Small Chests

### Medium Chests

### Large Chests

### Extra-Large Chests

## Shrines

## Statuses

Statuses are effects enemies and players might find themselves in.

### Chilled

Chilled is an effect caused by cold. The level of chilled stacks, so if someone with a chill status of '3' gets
hit by a cold attack that adds 2 more to the chilled status, their status will be '5' total. A chill status of 10 or
more causes the subject to freeze in place for the greatest number of seconds hit with and then their status resets. 
A chill status greater than 10 has no effect.

### Burning

Burrning is an effect caused by fire. Fire damage causes flames to spawn in the impact zone. Staying in that zone deals
a percentage of that damage per second, and the patch lasts a set amount of seconds.

## Levels

The elevators will be separated into levels. The starting levels 1-10 will be right next to the spawn. The higher levels
will be hidden behind harder and harder obbys with a level check barrier at the end. 

There will be 5 sets of elevators.
1. One will be the single player. One person sits down and a 10 second timer starts. If they click OK or the timer runs 
out they get teleported into a single player server and it empties for the next one.
2. Two will be two player. When the second person sits down a 15 second timer starts. If both click OK or both sit the
timer out they get teleported into a two-player server and it empties for the next two.
3. Two will be four player. Same, but with a 20 second timer when all 4 sit down.

Inside the elevator there will be a level to complete. Usually the level consists of solving a puzzle, defeating some
enemies, or both. The end of each level will have a boss who if defeated within a timer spawns 3 extra large chests. If
defeated after the timer, only 1 extra large chest.

The level can contain a hidden stockroom, where rare items can be found with higher frequency than the normal stockroom.
There could even be in-level stockroom exclusive gear, and the prices can be anywhere from 10-60% lower!

The level will use its tilesets to determine the challenges within, the baddies you'll face, and the ambiance of the
level.

The level can contain a number of chests. Small, medium, large, and extra large chests can be found. Large and extra 
large chests can be trapped. Some weapons may be able to detect and disarm traps.

The level can contain a number of shrines. These shrines have techno-babbly names but can grant all kinds of bonuses.
Some shrines can be trapped. Some weapons may be able to detect and disarm traps.

### Terminus

Terminus is the main lobby. There will be a stockroom where players can spend their nanites on boxes containing jewels,
runes, upgrades, and weapons. They can also manage their inventory and buildout here, to change their builds, cores and 
stat points. 

### Molten Core

### Chemistry Lab

### Overgrown Jungle Zoology Lab

### Classrooms

