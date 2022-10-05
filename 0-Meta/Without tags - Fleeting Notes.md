# Fleeting notes without tags

```dataview
list aliases
from "FleetingNotes"
where length(file.tags) = 0
sort file.ctime desc
```