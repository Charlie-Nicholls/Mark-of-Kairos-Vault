---
type: statblock
---
###### Last Breath of Tarhunz
<span class="sub2">:FasMapLocationDot: Environment </span>
___

```statblock
name: Last Breath of Tarhunz
source: Homebrew
size: Medium
type: elemental
subtype: ""
ac: 14
hp: 97
hit_dice: 13d10 + 26
speed: 50 ft., fly 50 ft. (hover)
stats:
  - 16
  - 19
  - 14
  - 10
  - 15
  - 11
skillsaves:
  - perception: 8
  - stealth: 10
damage_vulnerabilities: ""
damage_resistances: bludgeoning, piercing, slashing
damage_immunities: poison
condition_immunities: exhaustion, grappled, paralyzed, petrified, poisoned, prone, restrained, unconscious
senses: darkvision 60 ft., passive Perception 18
languages: Auran, understands Common but doesn't speak it
cr: "6"
bestiary: true
traits:
  - name: Air Form
    desc: The Last Breath of Tarhunz can enter a creature's space and stop there. It can move through a space as narrow as 1 inch without expending exra movement to do so.
  - name: Heart of the Storm
    desc: "At the start of the Last Breath of Tarhunz's turn roll a d6. On a 4-6 summon a Weakened Air Elemental. A maximum of 2 can exist at once and they die if the Last Breath of Tarhunz reaches 0 hit points."
actions:
  - name: Multiattack
    desc: The Last Breath of Tarhunz makes three Wind Swipe attacks.
    attack_bonus: 0
  - name: Wind Swipe
    desc: "Melee Attack Roll: +7, reach 5 ft. Hit: 11 (2d6 + 4) Force damage."
    attack_bonus: 7
    damage_dice: 2d6
    damage_bonus: 4
  - name: Tarhunz Final Scream
    desc: "*Constitution Saving Throw*: DC 14, one Large or smaller creatyre in the Last Breath of Tarhunz's space. *Failure:* 7 (1d8 + 3) Thunder damage, and the target has the Grappled condition (escape DC13). Until the grapple ends, the target can't cast spells with verbal components and takes 7 (2d6) Thunder damage at the start of the Last Breath of Tarhunz's turns."
