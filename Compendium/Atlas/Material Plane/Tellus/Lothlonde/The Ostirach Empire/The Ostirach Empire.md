---
type: territory
locations:
 - "[[Lothlonde]]"
displayLink: "[[The Ostirach Empire]]"
---

![[imgOstirachEmpire.jpg|banner p+cct]]

---

###### The Ostirach Empire
<span class="sub2">:FasChessRook: Kingdom</span>

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
>>FROM "Compendium/NPCs" AND [[The Ostirach Empire]] OR "Compendium/Party" AND [[The Ostirach Empire]] 
> 
>> [!example]- LOCATIONS
>>```dataview
LIST WITHOUT ID displayLink + " (" + type + ")"
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde/The Ostirach Empire" AND [[The Ostirach Empire]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[The Ostirach Empire]]
SORT file.ctime DESC