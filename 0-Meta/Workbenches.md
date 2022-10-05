# Workbenches
```dataviewjs
for (let group of dv.pages('#wb and !"Templates"').groupBy(p => p.tags)) {
	dv.table([group.key.split("/")[1], ""],
		group.rows
			.map(k => [k.file.link, k["aliases"]]))
}
```
