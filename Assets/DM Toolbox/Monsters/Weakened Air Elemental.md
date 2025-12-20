---
type: statblock
---
###### Last Breath of Tarhunz
<span class="sub2">:FasMapLocationDot: Environment </span>
___

```statblock
name: Weakened Air Elemental
source: Homebrew
size: Large
type: elemental
subtype: ""
alignment: neutral
ac: 15
hp: 40
speed: 10ft. fly 90 ft. (hover)
stats:
  - 14
  - 20
  - 14
  - 6
  - 10
  - 6
damage_vulnerabilities: ""
damage_resistances: lightning, thunder, bludgeoning, piercing, slashing
damage_immunities: poison
condition_immunities: exhaustion, grappled, paralyzed, petrified, poisoned, prone, restrained, unconscious
senses: darkvision 60 ft., passive Perception 10
languages: Auran
cr: "3"
bestiary: true
traits:
  - name: Air Form
    desc: The elemental can enter a hostile creature's space and stop there. It can move through a space as narrow as 1 inch wide without squeezing.
    attack_bonus: 0
actions:
  - name: Multiattack
    desc: The elemental makes two Thunderous Slam attacks.
    attack_bonus: 0
  - name: Thunderous Slam
    desc: "Melee Attack Roll: +6 to hit, reach 5 ft., one target. Hit: 10 (2d6 + 3) thunder damage."
    attack_bonus: 6
    damage_dice: 2d6
    damage_bonus: 3
  - name: Whirlwind (1/Day)
    desc: |-
      Each creature in the elemental's space must make a DC 13 Strength saving throw. On a failure, a target takes 15 (3d8 + 2) bludgeoning damage and is flung up 20 feet away from the elemental in a random direction and knocked prone. If a thrown target strikes an object, such as a wall or floor, the target takes 3 (1d6) bludgeoning damage for every 10 feet it was thrown. If the target is thrown at another creature, that creature must succeed on a DC 13 Dexterity saving throw or take the same damage and be knocked prone.
      If the saving throw is successful, the target takes half the bludgeoning damage and isn't flung away or knocked prone.
    attack_bonus: 0
```

