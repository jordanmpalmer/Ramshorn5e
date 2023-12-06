```dataviewjs
let input = {
  "query": 'TABLE without id file.link as NPC, race, sex, summary as "Summary" where type = "npc"',
  "filterColumnCount": 3,
  "markdownTable": false,
  "columnsWithoutFilters": ["Summary"],
  "filterCalloutColor": "blue",
  "its_cards": {
      "enabled": false,
      "columns": 3
  }
}
await dv.view("views/filtering_dv", input) 
```
![[Screenshot 2023-12-05 at 9.45.55 PM.png]]
![[Screenshot 2023-12-05 at 9.46.04 PM.png]]

![[272704618-c28662d9-a5b7-4b84-abed-85f06785ea78.gif]]

```
const page = dv.current()

async function getLocationNotes(parentLink) {
  const locations = [];
  const results = await dv.tryQuery('list from #location where parent_location = ' + parentLink);
  for (const result of results.values) {
    locations.push(result);
    const childLocations = await getLocationNotes(result);
    locations.push(...childLocations);
  }
  return locations;
}

let imageResPath = ""
if (page != null && page.image_link != null && page.image_link.path != null) {
    try {
    const imagePath = app.vault.getAbstractFileByPath(page.image_link.path)
    imageResPath = app.vault.getResourcePath(imagePath)
    } catch (e) {
    // image doesnt exist...
    }
}

const locationNotes = await getLocationNotes(dv.current().file.link);

dv.span(`
> [!infobox|no-table-header]
> ## \`=this.name\`
> \`$= dv.el("img", "test", { attr: {"src": "${imageResPath}", alt: "center cover wm-small"}})\`
> 
> |  |  | 
> |-|-|
> | Leadership | \`=this.leaderships\` |
> | NPCs | \`=this.npcs\` |
> | Location Type | \`=this.subtype\` |
> | Location Parent | \`=this.parent_location\` |
> | Relative Locations | \`$= if (dv.current().parent_location) { dv.span((await dv.tryQuery('list rows.file.link where parent_location = ' + dv.current().parent_location + ' group by parent_location')).values) }\` |
> | Location Children | \`$= dv.span((await dv.tryQuery('list from #location sort locationNumber, file.name where parent_location = ' + dv.current().file.link)).values)\` |


# \`=this.name\`

> [!summary]
> \`=this.summary\`

`)

dv.span("> [!example]- All children " + locationNotes.map(n => "\n> - " + n).join(""));
```