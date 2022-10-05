# Hubs
## Level-1

```dataview
table file.aliases AS "Name"
from !"Templates"
where hub-level = 1
sort file.aliases
```

## Level-2

```dataview
table file.aliases AS "Name"
from !"Templates"
where hub-level = 2
sort file.aliases
```