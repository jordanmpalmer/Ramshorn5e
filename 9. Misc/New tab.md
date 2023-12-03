---
banner: "![[DnDBannerClasses.png]]"
---

|![[Minastria.png\|hsmall]] | Ramshorn     | Character Sheet | DM Screen |
| ------------- | ------------ | --------------- | --------- |
| [[Minastria]] | [[Ramshorn]] |                 |           |

######
```dataview
table Player, Race, Class, Level, tags
from "2. PCs"
where status="active"
where type="PC"
```

######
```dataview  
TABLE WITHOUT ID  
link(file.path, file.folder + " / " + file.name) AS "Note",  
file.mtime AS "Last modified"  
FROM "/"  
WHERE file.mtime >= date(today) - dur(30 days)  
AND file.name != this.file.name  
AND !contains(file.path, "z_Assets")  
AND !contains(file.path, "Inline Scripts")  
AND !contains(file.path, "z_Templates")  
AND !contains(file.path, "daily notes")  
AND !contains(file.path, "BRAT")  
SORT file.mtime DESC  
LIMIT 10  
```




