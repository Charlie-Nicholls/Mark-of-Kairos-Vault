---
cssClasses: index
displayLink: "[[NPCs]]"
---
###### <span class="head">Non Player Characters</span> 

### Major NPCs

```dataviewjs
// Set path and class
const vault = this.app.vault.adapter.getResourcePath("").split("?")[0];
dv.container.className += ' hideSort cards cards-cover cards-1-1';

// Display PC card table
dv.table(["cover", "name"],
  dv.pages(`"Compendium/NPCs/Major NPCs"`)
  .sort(page => page.file.name, "asc")
    .map(p => [
      `![](${vault}/${p.cover})`,
      p.displayLink,
    ])
);
```

### Moderate NPCs

```dataviewjs
// Set path and class
const vault = this.app.vault.adapter.getResourcePath("").split("?")[0];
dv.container.className += ' hideSort cards cards-cover cards-1-1';

// Display PC card table
dv.table(["cover", "name"],
  dv.pages(`"Compendium/NPCs/Moderate NPCs"`)
  .sort(page => page.file.name, "asc")
    .map(p => [
      `![](${vault}/${p.cover})`,
      p.displayLink,
    ])
);
```

### Minor NPCs

```dataviewjs
// Set path and class
const vault = this.app.vault.adapter.getResourcePath("").split("?")[0];
dv.container.className += ' hideSort cards cards-cover cards-1-1';

// Display PC card table
dv.table(["cover", "name"],
  dv.pages(`"Compendium/NPCs/Minor NPCs"`)
  .sort(page => page.file.name, "asc")
    .map(p => [
      `![](${vault}/${p.cover})`,
      p.displayLink,
    ])
);
```