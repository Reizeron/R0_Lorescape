```dataview
TABLE file.inlinks as Backlinks, length(file.inlinks) as Total
FROM "Topics"
SORT length(file.inlinks) DESC
```
