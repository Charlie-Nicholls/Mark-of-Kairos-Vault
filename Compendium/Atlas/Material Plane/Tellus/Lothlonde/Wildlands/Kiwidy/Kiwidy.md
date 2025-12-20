---
type: locale
locations:
 - "[[Wildlands]]"
aliases: ["Silent City of Kiwidy"]
displayLink: "[[Kiwidy]]"
---

![[imgSilentCityOfKiwidy.png|banner p+cb]]
###### Kiwidy
<span class="sub2">:FasCity: City</span>

---

> [!boxed|no-t]
> Introduction for players
>^IntroText

### Description
Known as the 'Silent City of Kiwidy'...

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
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde/Wildlands/Kiwidy" AND [[#]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[#]]
SORT file.ctime DESC