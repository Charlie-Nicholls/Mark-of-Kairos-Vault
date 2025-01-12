---
type: realm
locations:
 - "[[Material Plane]]"
displayLink: "[[Tellus]]"
---

![[imgTellus.jpg|banner]]

---

###### Tellus
<span class="sub2">:RiGlobalLine: Realm (world)</span>

---

> [!recite|clean no-t]
>	Introduction for players
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
>>```dataview
LIST WITHOUT ID displayLink
FROM "Compendium/Atlas/Material Plane/Tellus" AND [[#]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[#]]
SORT file.ctime DESC