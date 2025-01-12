---
type: locale
locations:
 - "[[Camarath]]"
displayLink: "[[Sentry District]]"
---

![[banner.jpg|banner]]
###### Sentry District
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
>>FROM "Compendium/NPCs" AND [[Sentry District]] OR "Compendium/Party" AND [[Sentry District]] 
> 
>> [!example]- LOCATIONS
>>```dataview
LIST WITHOUT ID displayLink
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde/Hestrela/Camarath/Sentry District" AND [[Sentry District]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[Sentry District]]
SORT file.ctime DESC