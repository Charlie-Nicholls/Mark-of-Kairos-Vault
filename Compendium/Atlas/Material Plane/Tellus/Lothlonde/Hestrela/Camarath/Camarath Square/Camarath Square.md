---
type: locale
locations:
 - "[[Camarath]]"
displayLink: "[[Camarath Square]]"
---

![[banner.jpg|banner]]
###### Camarath Square
<span class="sub2">:FasCircleQuestion: District</span>

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
>>FROM "Compendium/NPCs" AND [[Camarath Square]] OR "Compendium/Party" AND [[Camarath Square]] 
> 
>> [!example]- LOCATIONS
>>```dataview
LIST WITHOUT ID displayLink
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde/Hestrela/Camarath/Camarath Square" AND [[Camarath Square]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[Camarath Square]]
SORT file.ctime DESC