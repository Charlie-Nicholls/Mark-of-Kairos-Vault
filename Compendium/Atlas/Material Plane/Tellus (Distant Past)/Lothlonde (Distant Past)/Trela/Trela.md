---
type: territory
locations:
 - "[[Lothlonde (Distant Past)]]"
displayLink: "[[Trela]]"
---

![[banner.jpg|banner]]

---

###### Trela
<span class="sub2">:FasChessRook: Kingdom</span>

---

> [!boxed|no-t]
> Introduction for players
>^IntroText

### Description
Description of Territory

---

> [!column|flex 3]
>> [!hint]-  NPCs
>>```dataview
LIST WITHOUT ID displayLink
FROM "Compendium/NPCs" AND [[#]] OR "Compendium/Party" AND [[#]]```
> 
>> [!example]- LOCATIONS
>>```dataview
LIST WITHOUT ID displayLink + " (" + type + ")"
FROM "Compendium/Atlas/Material Plane/Tellus (Distant Past)/Lothlonde (Distant Past)/Trela" AND [[#]]
WHERE file.name != this.file.name
SORT file.name ASC```
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[#]]
SORT file.ctime DESC```