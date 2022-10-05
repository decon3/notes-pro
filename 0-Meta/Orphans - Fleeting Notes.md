# Orphaned Fleeting Notes

```dataview
list aliases
from "FleetingNotes"
where length(file.inlinks) = 0 and length(file.outlinks) = 0
sort file.ctime desc
```
