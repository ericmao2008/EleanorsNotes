
## Microfiction

```dataview
table status, file.size, protagonist, location, year, pitch
from "80 Stories"
where contains(length, "lash")
sort status desc
```

```dataview
table status, mentions, protagonist, location, year, pitch
from "80 Stories"
where contains(length, "icro")
sort status desc
```