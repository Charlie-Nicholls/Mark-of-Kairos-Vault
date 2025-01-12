---
type: realm
locations:
 - "[[Material Plane]]"
displayLink: "[[The Dark Storm]]"
aliases: ["Howling Madness", "Siren's Void"]
---

![[imgTheDarkStorm.jpg|p+ct banner]]

---

###### The Dark Storm
<span class="sub2">:RiGlobalLine: Realm (world)</span>

---
> [!recite|clean no-t]
>	Some call it the 'Howling Madness', some the 'Siren's Void', 'The Dark Storm', or simply 'Hell'.
>^IntroText

### Description
Description of realm

---

> [!column|flex 3]
>> [!hint]-  NPCs
>>```dataview
LIST WITHOUT ID displayLink
FROM "Compendium/NPCs" AND [[#]] OR "Compendium/Party" AND [[#]] 
>
>> [!example]- LOCATIONS
LIST WITHOUT ID displayLink
FROM "Compendium/Atlas/Material Plane/The Dark Storm" AND [[#]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[#]]
SORT file.ctime DESC