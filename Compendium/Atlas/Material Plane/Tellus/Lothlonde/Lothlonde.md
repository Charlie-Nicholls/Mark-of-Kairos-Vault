---
type: continent
locations:
 - "[[Tellus]]"
displayLink: "[[Lothlonde]]"
---

![[imgLothlondeMap.png|banner]]
###### Lothlonde
<span class="sub2">:FasEarthAmericas: Continent</span>

---

> [!boxed|no-t]
> Introduction for players
>^IntroText
	
### Description
Description of continent

### Map
```leaflet
id: lothlonde-map
image: [[mapLothlondeCenter.jpg]]
height: 600px
lat: 50%
long: 50%
minZoom: 7.66
maxZoom: 10.06
defaultZoom: 7.66
zoomDelta: 0.5
unit: meters
recenter: true
scale: 1
noUI: true
lock: true

```

---

> [!column|flex 3]
>> [!hint]-  NPCs
>>```dataview
>>LIST WITHOUT ID displayLink
>>FROM "Compendium/NPCs" AND [[Lothlonde]] OR "Compendium/Party" AND [[Lothlonde]] 
> 
>> [!example]- LOCATIONS
>>```dataview
LIST WITHOUT ID displayLink
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde" AND [[Lothlonde]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[Lothlonde]]
SORT file.ctime DESC