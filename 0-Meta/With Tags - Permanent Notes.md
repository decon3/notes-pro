# Permanent notes with tags

```dataview
list aliases
from "PermanentNotes"
where length(file.tags) > 0
and !hub-level
sort file.ctime desc
```