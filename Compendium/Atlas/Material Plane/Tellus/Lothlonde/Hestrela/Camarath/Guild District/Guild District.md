---
type: locale
locations:
 - "[[Camarath]]"
displayLink: "[[Guild District]]"
---

![[banner.jpg|banner]]
###### Guild District
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
>>FROM "Compendium/NPCs" AND [[Guild District]] OR "Compendium/Party" AND [[Guild District]] 
> 
>> [!example]- LOCATIONS
>>```dataview
LIST WITHOUT ID displayLink
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde/Hestrela/Camarath/Guild District" AND [[Guild District]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[Guild District]]
SORT file.ctime DESC