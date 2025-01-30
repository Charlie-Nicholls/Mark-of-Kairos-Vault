```dataviewjs
let pages = dv.pages('"Compendium/Atlas"').sort(p => p.number, "asc"); 
let places = [];
for (let i=0; i < pages.length; i++) {
	places.push(`- [ ] [[${pages[i].file.name}]]`);
	}
dv.list(places)
```