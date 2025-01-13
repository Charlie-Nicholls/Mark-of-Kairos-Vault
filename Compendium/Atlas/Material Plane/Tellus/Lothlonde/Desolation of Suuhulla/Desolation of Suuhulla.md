---
type: territory
locations:
 - "[[Lothlonde]]"
displayLink: "[[Desolation of Suuhulla]]"
---

![[imgDesolationOfSuuhulla.png|banner p+tcc]]

---

###### Desolation of Suuhulla
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
LIST WITHOUT ID displayLink
FROM "Compendium/NPCs" AND [[#]] OR "Compendium/Party" AND [[#]] 
> 
>> [!example]- LOCATIONS
>>```dataview
LIST WITHOUT ID displayLink + " (" + type + ")"
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde/Desolation of Suuhulla" AND [[#]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[#]]
SORT file.ctime DESC