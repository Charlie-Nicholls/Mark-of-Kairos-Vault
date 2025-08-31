---
type: statblock
---
###### Ocean Environment
<span class="sub2">:FasMapLocationDot: Environment </span>
___

```statblock
name: Ocean
tier: "2"
layout: Daggerheart Environment
type: Traversal
description: Water stretches out as far as the eye can see, stormy waters threaten sailors while creatures unknown lurk beneath the surface.
impulses: Test stamina and navigational skills, rock the boat, monsters seek to sink ships
difficulty: "14"
potential_adversaries: Pirate Ship (Pirate Captain, Pirate Raiders, Pirate Tough), Electric Eels, Shark, Siren
feats:

  - name: Sleepless Nights - Passive
    text: |-
      It is not possibly to truly rest during the harsh life on the sea. PCs may choose 1 fewer Downtime Actions during rests.
        *How do you help with navigation? Directly or by helping with life on the ship in other ways? How are you spending your free time during the long voyage?*
  - name: Ocean Navigation - Passive
    text: |-
      Crossing the ocean requires the party to complete a Progress Countdown (number of hexes moved), by making Navigation rolls every 6 hours. A Navigation roll with fear immediately acivate the Worsen Weather, High Seas or Siren's Lure feature without the need to spend a fear. On a Navigation roll with Hope, the PC can choose to spend a Hope to reduce the Weather Difficulty by 1.

        *How do you help with navigation? Directly or by helping with life on the ship in other ways? How are you spending your free time during the long voyage?*
        
  - name: Weather Effects - Passive
    text: |-
      Choose a Weather Difficulty to start the journey at, by default 2. Waiting for 6 hours without a Navigation check causes the Weather Difficulty to change according to a d6 roll as follows: 
      1: +1 (max 4), 2-4: +0, 5-6: -1. 
      Each weather has the following effect:
      1. Clear Skies - Advantage on Navigation rolls
      2. Rainy Day - **Mark a Stress** on a Navigation roll with Fear.
      3. Foggy Waters - Disadvantage on Navigation rolls
      4. Stormy Seas - Players must **Mark a Stress** to make or help with a Navigation rolls. Failure with Fear blows you off course, increasing the Progress Countdown by 1.
      5. Hurricane Season (Phase Change) - A Hurricane rolls in, replace this with the Hurricane environment. This cannot be activated more than once.

        *What questions should go here? What questions should go here?*
        
        
  - name: Worsen Weather - Action
    text: |-
      *Spend a Fear* to increase the Weather Difficulty by 1.

        *What questions should go here? What questions should go here?*
        
  - name: High Seas - Action
    text: |-
      *Spend a Fear* to cause a Pirate Ship containing a Pirate Captain, 2 Pirate Bruisers and 3 Pirate Hordes to appear at Very Far distance.

        *Does the Pirate Ship try to board them? Do the players recognise it for what it is? Do the players flee the ship or try to fight it?*
        
  - name: Siren's Lure - Action
    text: |-
      Have an alluring Siren appear at the side of the ship and try to charm the PCs. *Spend a Fear* when two Sharks under her spell pretend to attack her and drag her underwater attempting to lure the PCs into jumping in to rescue her. If any do, the Siren and 2 Sharks attempt to attack and eat the PC.

        *How does the Siren attempt to charm the Players? What would she appear like to her target? How good is her acting when being 'attacked'?*
source: Homebrew
```

