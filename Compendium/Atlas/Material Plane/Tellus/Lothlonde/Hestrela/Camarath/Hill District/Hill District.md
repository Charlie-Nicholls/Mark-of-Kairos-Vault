---
type: locale
locations:
 - "[[Camarath]]"
displayLink: "[[Hill District]]"
---

![[banner.jpg|banner]]
###### Hill District
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
>>FROM "Compendium/NPCs" AND [[Hill District]] OR "Compendium/Party" AND [[Hill District]] 
> 
>> [!example]- LOCATIONS
>>```dataview
LIST WITHOUT ID displayLink
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde/Hestrela/Camarath/Hill District" AND [[Hill District]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[Hill District]]
SORT file.ctime DESC