---
sessions: 26
---
![[DM Screen.png]]
>[!cards|5] 
>**[[Cedrick Ballard|Cedrick]]**
>![[Cedrick.jpg|sban hw-med cover]]
>
>**[[Dane Ogden|Dane]]**
>![[Dane.png|sban hw-med cover]]
>
>**[[Dramus Ardor|Dramus]]**
>![[Dramus.webp|sban hw-med cover]]
>
>**[[Sol Siofra|Sol]]**
>![[z_Assets/NPC_Placeholder.png|Sol]]
>
>**[[Zion Dawnbreak|Zion]]**
>![[Zion.png|sban hw-med cover]]

>[!info|bg-gray c-blue] GM Tipp
> Test of the GM tip

```dataviewjs 
const dice = window.app.plugins.plugins['obsidian-dice-roller']; 
const roll = await dice.parseDice('[](z_Assets/z_GM Screen/Random Notes/Random Notes.md)|line', ''); 
dv.span(roll.result); 

	[!columns|flex 3 no-t] 
		[!warning|no-i] Recent Notes

dataview
		TABLE WITHOUT ID
		Note,
		dateformat(file.mtime, "dd.MM.yyyy") AS "<div>Datum</div>"
		FROM "/"
		WHERE file.mtime >= date(today) - dur(30 days)
		AND file.name != this.file.name
		AND !contains(file.path, "z_Assets")
		SORT file.mtime DESC
		FLATTEN "[[" + file.path + "|" + truncate(file.name, 21) + "]]" as Note
		LIMIT 6

		[!warning|no-i] Session Notes

		TABLE WITHOUT ID link(file.name) AS "Session", 
		dateformat(Datum, "dd.MM.yyyy") AS "<div>Datum</div>"
		from #Session 
		WHERE !contains(file.path, "z_Assets") 
		SORT Datum DESC
		limit 6 
				
		[!warning|no-i] Kalender

calendarium

	[!columns|flex 2 no-t] 
		[!warning|no-i] Aktive Quests



dataview
		TABLE without ID file.link as "Quests", Ort
		from #Quest 
		WHERE !contains(file.path, "z_Assets") 
		WHERE contains(Status, "Aktiv")

[!warning|no-i]- Karte
![[Karte - Schwertküste|no-h no-t no-link clean]]

		[!columns|flex 3 no-t] 
		[!warning|no-i] To-Do
		- [ ] Fraktion Template 
		- [x] Fronten Template 
		- [x] Quests Template 
		- [ ] Session Notes Template
```





