# Created
```dataview
TABLE aliases as Name, file.cday as On
FROM ""
WHERE date(now) - file.ctime <= dur(15 days)
SORT file.ctime desc LIMIT 50
```

# Edited
```dataview
TABLE aliases as Name, file.mday as On
FROM ""
WHERE date(now) - file.mtime <= dur(15 days) and file.name != "Recent notes.md"
SORT file.mtime desc LIMIT 50
```
