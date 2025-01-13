---
cssClasses: index
displayLink: "[[Session Notes]]"
alias: "Campaign Story"
---
###### <span class="head">Campaign Story</span> 
![[campaign.jpg|banner]]

 ### :FasBook: Arc One - The Mark of Kairos
 
```dataviewjs
let pages = dv.pages('"Session Notes"').sort(p => p.number, "asc"); 
let chapters = [];
for (let i=0; i < pages.length; i++) {
	if (pages[i].arc == 1) {
		chapters.push(`[[${pages[i].file.name}|Part ${pages[i].number}: ${pages[i].alias}]]`);
		}
	}
dv.list(chapters)
```

<br>

### :FasBook: Arc Two - The Mark of Vacuuous

```dataviewjs
let pages = dv.pages('"Session Notes"').sort(p => p.number, "asc"); 
let chapters = [];
for (let i=0; i < pages.length; i++) {
	if (pages[i].arc == 2) {
		chapters.push(`[[${pages[i].file.name}|Part ${pages[i].number}: ${pages[i].alias}]]`);
		}
	}
dv.list(chapters)
```
