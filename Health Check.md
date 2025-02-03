---
tags:
  - Index
---

## Orphan Notes
```dataview
TABLE file.name AS "Orphan Notes"
FROM ""
WHERE length(file.inlinks) = 0 AND length(file.outlinks) = 0
SORT file.ctime ASC
```

### Empty Notes

```dataview
TABLE file.name AS "Empty Notes"
FROM ""
WHERE file.size = 0
SORT file.ctime ASC
```

