<%*
// ###########################################################
//                        Helper Functions
// ###########################################################

// Convert string to camelCase
function toCamelCase(str) {
  return str
    .replace(/(?:^\w|[A-Z]|\b\w|\s+|[-_])/g, (match, index) =>
      index === 0 ? match.toLowerCase() : match.toUpperCase()
    )
    .replace(/[\s-_]+/g, '');
}

// ###########################################################
//                        Main Code Section
// ###########################################################

// Call modal form & declare variables
const result = await MF.openForm('NOTE');
const date = result.Date.value;
const title = result.Title.value;
const location = result.Location.value ? result.Location.value.map(value => `- "[[${value}]]"`).join("\n") : '';
const arc = result.Arc.value;
const number = result.Number.value;
const name = `Arc ${arc} Session ${number}`;

if (result.status === 'ok') {

    // Rename file & open in new tab; Fire toast notification
    await tp.file.rename(name);
    await app.workspace.getLeaf(true).openFile(tp.file.find_tfile(name));
    new Notice().noticeEl.innerHTML = `<span style="color: green; font-weight: bold;">Finished!</span><br>New note <span style="text-decoration: underline;">${name}</span> added`;

} else {

    // Fire toast notification & exit templater
    new Notice().noticeEl.innerHTML = `<span style="color: red; font-weight: bold;">Cancelled:</span><br>Session note has not been added`;
    return;
}
_%>

---
type: notes
arc: <% arc %>
number: <% number %>
date: <% date %>
alias: "<% title %>"
displayLink: "[[<% name %>|<% arc %>.<% number %>: <% title %>]]"
---

![[session.png|banner]]
###### Arc `=this.arc` Session `=this.number`: `=this.alias`
<span class="sub2">:FasCalendar: `=this.date` </span>
___

> [!column|flex 3]
> 
>> [!info|flex]- NPCS:
>> - [[Characters]]
>
>> [!example|flex]- LOCATIONS:
>> <% location ? location : ' - '%>
>
>> [!important|flex]- QUESTS:
>> - [[Quests]]

---


### Plan
> [!recite|nbrd no-i] Fear Tracker
> <input type="checkbox"> <input type="checkbox"> <input type="checkbox"> <input type="checkbox"> <input type="checkbox"> <input type="checkbox"> <input type="checkbox"> <input type="checkbox"> <input type="checkbox"> <input type="checkbox"> <input type="checkbox"> <input type="checkbox">

Plan for the session here.

### Notes
- Live notes from the session here.

### Summary
Summary of the important points from the session here.


