---
aliases:
---
```dataview
TABLE file.name as Track, length(filter(file.tasks, (t) => t.completed)) AS "Completed Tasks", length(filter(file.tasks, (t) => !t.completed)) AS "Incomplete Tasks" FROM "" WHERE file.name = "Associate Data Engineer in SQL"
```
