---
type: locale
locations:
 - "[[Camarath]]"
displayLink: "[[Hawker's Caverns]]"
---

![[imgHawkersCaverns.jpg|banner p+ccb]]
###### Hawker's Caverns
<span class="sub2">:FasMound: Cave</span>

---

> [!recite|clean no-t]
>	Introduction for players
>^IntroText

### Description
Description of location

---

> [!column|flex 3]
>> [!hint]-  NPCs
>>```dataview
>>LIST WITHOUT ID displayLink
>>FROM "Compendium/NPCs" AND [[Hawker's Caverns]] OR "Compendium/Party" AND [[Hawker's Caverns]] 
> 
>> [!example]- LOCATIONS
>>```dataview
LIST WITHOUT ID displayLink
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde/Hestrela/Camarath/Hawker's Caverns" AND [[Hawker's Caverns]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[Hawker's Caverns]]
SORT file.ctime DESC