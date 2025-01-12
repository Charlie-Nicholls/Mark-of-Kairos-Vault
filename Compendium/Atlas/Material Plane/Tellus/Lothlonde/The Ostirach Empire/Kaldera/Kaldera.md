---
type: locale
locations:
 - "[[The Ostirach Empire]]"
displayLink: "[[Kaldera]]"
---

![[imgKaldera.jpg|banner]]
###### Kaldera
<span class="sub2">:FasCity: City</span>

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
>>FROM "Compendium/NPCs" AND [[Kaldera]] OR "Compendium/Party" AND [[Kaldera]] 
> 
>> [!example]- LOCATIONS
>>```dataview
LIST WITHOUT ID displayLink
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde/The Ostirach Empire/Kaldera" AND [[Kaldera]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[Kaldera]]
SORT file.ctime DESC