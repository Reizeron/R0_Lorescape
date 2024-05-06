```dataview
TABLE without id 
out AS "Uncreated files", origin as "Origin", linkCount as "Link Count"
FLATTEN file.outlinks as out
WHERE !(out.file) AND !contains(meta(out).path, "/") AND !contains(file.tags, "todo")
GROUP BY out
FLATTEN length(rows.out) as linkCount
FLATTEN rows.file.link as origin
SORT linkCount DESC
Limit 200
```
