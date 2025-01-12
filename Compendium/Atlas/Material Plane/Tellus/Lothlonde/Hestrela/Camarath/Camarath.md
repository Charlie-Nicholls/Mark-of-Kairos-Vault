---
type: locale
locations:
 - "[[Hestrela]]"
displayLink: "[[Camarath]]"
---

![[imgCamarath.jpg|p+cbb banner]]
###### Camarath
<span class="sub2">:FasCity: City</span>

---

> [!recite|clean no-t]
>	Introduction for players
>^IntroText

### Description
Description of location

### Map
```leaflet
id: camarath-map
image: [[imgCamarathMap.png]]
height: 600px
lat: 50%
long: 50%
minZoom: 7
maxZoom: 10
defaultZoom: 7
zoomDelta: 0.5
unit: meters
recenter: true
scale: 1
noUI: true
lock: true
marker: default,-0.6875,3.4296735141424985,Storm Haven,,,
marker: default,-1.2799072265625,4.545661027568922,Hawker's Caverns,,,
marker: default,-1.9375,3.3593694056569996,Guild District,,,
marker: default,-2.0859375,2.8749944056569996,Noble's District,,,
marker: default,-2.03125,2.265625,Camarath Square,,,
marker: default,-2.6171875,1.5859263113139992,Monument District,,,
marker: default,-2.7265625,2.2890652971714998,Scholar's District,,,
marker: default,-3.5625,2.6484458915145,Hill District,,,
marker: default,-3.9921875,2.1875055943430004,Sentry District,,,
marker: default,-2.3125,4.4452034103114935,Beggar's Docks,,,
```


<br>

---

> [!column|flex 3]
>> [!hint]-  NPCs
>>```dataview
LIST WITHOUT ID displayLink
FROM "Compendium/NPCs" AND [[Camarath]] OR "Compendium/Party" AND [[Camarath]] 
> 
>> [!example]- LOCATIONS
>>```dataview
LIST WITHOUT ID displayLink
FROM "Compendium/Atlas/Material Plane/Tellus/Lothlonde/Hestrela/Camarath" AND [[Camarath]]
WHERE file.name != this.file.name
SORT file.name ASC
>
>> [!note]- HISTORY
>>```dataview
LIST WITHOUT ID displayLink
FROM "Session Notes" AND [[Camarath]]
SORT file.ctime DESC