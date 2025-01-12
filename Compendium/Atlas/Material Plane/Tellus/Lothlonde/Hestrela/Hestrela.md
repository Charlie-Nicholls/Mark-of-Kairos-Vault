---
type: territory
locations:
 - "[[Lothlonde]]"
displayLink: "[[Hestrela]]"
---

![[imgHestrela.jpg|banner]]

---

###### Hestrela
<span class="sub2">:FasMap: General Region</span>

---

> [!recite|clean no-t]
>	Introduction for players
>^IntroText

### Description
Description of Territory

---

> [!column|flex 3]
>> [!hint]-  NPCs
>>```dataview
>>LIST WITHOUT ID displayLink
>>FROM "Compendium/NPCs" AND [[Hestrela]] OR "Compendium/Party" AND [[Hestrela]] 
> 
>> [!example]- LOCATIONS
>>```dataview
LIST WITHOUT ID displayLink + " (" + type + ")"
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde/Hestrela" AND [[Hestrela]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[Hestrela]]
SORT file.ctime DESC