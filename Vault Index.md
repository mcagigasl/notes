
```dataviewjs
dv.table(["Note", "Description"], dv.pages("#Index") .map(p => [p.file.link, p.Description]) );
```
