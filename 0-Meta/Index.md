# Index
<!--
```dataview
TABLE split(file.tags[1], "/")[1] AS "Tags",
      aliases AS "Aliases"
 FROM #index
WHERE contains(file.tags, "/")
SORT file.tags
```
-->

```dataviewjs
for (let group of dv.pages('#index').groupBy(p => p.tags)) {
	dv.table([group.key.split("/")[1]],
		group.rows
			.map(k => [k.file.link + " . . . " + k["aliases"]]))
}
```
