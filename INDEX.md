---
cssClasses: index
---
###### <span class="head">The Mark of Kairos</span> 
![[campaign.jpg|banner]]

```dataviewjs
// Set path and class
const vault = this.app.vault.adapter.getResourcePath("").split("?")[0];
dv.container.className += ' hideSort cards cards-cover cards-1-1';

// Display PC card table
dv.table(["cover", "name"],
  dv.pages(`"Compendium/Party/Player Characters"|"Compendium/NPCs/Major NPCs"`)
  .sort(page => page.file.name, "asc")
    .map(p => [
      `![](${vault}/${p.cover})`, // For image link use: [![](${vault}/${p.cover})](<${p.file.name}#${p.file.name}>)
      p.displayLink,
      obsidian.Platform.isMobile ? `<center> :FasUserGroup: ${p.race}<br>:RiSwordFill: ${p.class} </center>` : `<center> :FasUserGroup: ${p.race} / :RiSwordFill: ${p.class} </center>`
    ])
);

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

> [!session]-  [[Session Notes]]<br><span class="sub">Summaries, Transcripts, & Notes</span>
> ```dataviewjs
> dv.container.className += ' listMe';
> let pages = dv.pages('"Session Notes"').sort(p => p.date, "desc");  
> dv.table(["Date"], pages.map(page => [`- ${page.displayLink}`]));
> ```
> `BUTTON[note]`

> [!npc]-   [[NPCs]]<br><span class="sub">Non-Player Characters</span>
> ```dataviewjs
> dv.container.className += ' listMe';
> dv.el("b", "Major NPCs")
> let major = dv.pages('"Compendium/NPCs/Major NPCs"').sort(p => p.file.name, "asc");  
> dv.table(["Name"], major.map(page => [`- ${page.displayLink}`]));
> dv.el("b", "Moderate NPCs")
> let moderate = dv.pages('"Compendium/NPCs/Moderate NPCs"').sort(p => p.file.name, "asc");  
> dv.table(["Name"], moderate.map(page => [`- ${page.displayLink}`]));
> dv.el("b", "Minor NPCs")
> let minor = dv.pages('"Compendium/NPCs/Minor NPCs"').sort(p => p.file.name, "asc");  
> dv.table(["Name"], minor.map(page => [`- ${page.displayLink}`]));
> ```
> `BUTTON[npc]`

> [!agenda]-  The Party<br><span class="sub">Objectives, Players, & Quests</span>
>```dataviewjs
> dv.container.className += ' listMe';
> let pages = dv.pages('"Compendium/Party/Quests"').sort(p => p.file.name, "asc");
> dv.table(["Name", "Status"], pages.map(page => {
> const questStatusTerms = ["completed", "abandoned", "failed", "ongoing", "pending"];
> let status = questStatusTerms.find(term => page.status && page.status.includes(term));
> status = status ? `(${status.replace("quest/", "")})` : "";
> return [`- ${page.displayLink} ${status}`, status];
> }));
> ```
> `BUTTON[pc]` `BUTTON[quest]`

> [!genloc]-  Locations<br><span class="sub">Countries, Settlements, & Topography</span>
> ```dataviewjs
> dv.container.className += ' listMe';
> let pages = dv.pages('"Compendium/Atlas"').sort(p => p.file.name, "asc");  
> dv.table(["Name", "Type"], pages.map(page => [`- ${page.displayLink} (${page.type})`, page.type]));
> ```
>`BUTTON[plane, realm, continent, territory, province, locale, landmark]`

> [!lore]-  Lore & Mythos<br><span class="sub">Factions, Gods, Relics, & More</span> 
> ```dataviewjs
> dv.container.className += ' listMe';
> let pages = dv.pages('"Compendium/Lore"').sort(p => p.file.name, "asc");  
> dv.table(["Name", "Type"], pages.map(page => [`- ${page.displayLink} (${page.type})`, page.type]));
> ```
> `BUTTON[deity, event, object, org]`