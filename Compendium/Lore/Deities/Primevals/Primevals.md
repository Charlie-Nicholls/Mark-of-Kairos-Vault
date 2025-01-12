---
type: lore
displayLink: "[[Primevals]]"
---

###### Primevals
<span class="sub2">:LiScrollText: Lore</span>
___

```dataviewjs
// Set path and class
const vault = this.app.vault.adapter.getResourcePath("").split("?")[0];
dv.container.className += ' hideSort cards cards-cover cards-1-1';

// Display Primevals card table
dv.table(["cover", "name", "details"],
  dv.pages(`"Compendium/Lore/Deities/Primevals/Kairos" | "Compendium/Lore/Deities/Primevals/Vacuuous" | "Compendium/Lore/Deities/Primevals/Diracmi" | "Compendium/Lore/Deities/Primevals/Scathach"`)
  .sort(page => page.file.name, "asc")
    .map(p => [
      `![](${vault}/${p.cover})`,
      p.displayLink,
      obsidian.Platform.isMobile ? `<center> :LiStars: ${p.domains} </center>` : `<center> :LiStars: ${p.domains} </center>`
    ])
);
```

---

	Introduction for players

### Description
Description of the  lore, Primevals.

---

>>[!hint]- PEOPLE
>>```dataview
>>LIST WITHOUT ID displayLink
>FROM "Compendium/NPCs" AND [[Primevals]] OR "Compendium/Party/Player Characters" AND [[Primevals]]
>
>>[!note]- DEITIES
>>```dataview
>LIST WITHOUT ID displayLink
>FROM "Compendium/Lore/Deities/Primevals"
>WHERE file.name != this.file.name
>SORT file.name ASC