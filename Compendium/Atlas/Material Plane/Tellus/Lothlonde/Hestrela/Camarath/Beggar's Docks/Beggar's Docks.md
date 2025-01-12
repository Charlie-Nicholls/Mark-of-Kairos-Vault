---
type: locale
locations:
 - "[[Camarath]]"
displayLink: "[[Beggar's Docks]]"
---

![[imgCamarathDocks.jpg|p+b banner]]
###### Beggar's Docks
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
>>FROM "Compendium/NPCs" AND [[Beggar's Docks]] OR "Compendium/Party" AND [[Beggar's Docks]] 
> 
>> [!example]- LOCATIONS
>>```dataview
LIST WITHOUT ID displayLink
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde/Hestrela/Camarath/Beggar's Docks" AND [[Beggar's Docks]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[Beggar's Docks]]
SORT file.ctime DESC