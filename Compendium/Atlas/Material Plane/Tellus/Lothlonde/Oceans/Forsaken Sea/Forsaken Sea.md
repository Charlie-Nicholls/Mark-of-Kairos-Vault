---
type: ocean
locations:
 - "[[Lothlonde]]"
displayLink: "[[Forsaken Sea]]"
---

![[banner.jpg|banner]]
###### Forsaken Sea
<span class="sub2">:FasWater: Ocean</span>

---

> [!boxed|no-t]
> Introduction for players
>^IntroText
	
### Description
Connects [[Camarath]] to the [[Wildlands]] in the south and the [[Desolation of Suuhulla]] in the north. Named by the [[Hestrela|Hestrelan's]] as crossing it leads you away from the lands blessed by the gods into the lands they forsake. 

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
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde/Forsaken Sea" AND [[#]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[#]]
SORT file.ctime DESC