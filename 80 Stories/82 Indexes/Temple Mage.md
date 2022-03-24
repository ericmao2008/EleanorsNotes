---
universe: "Verraine"
year: "350 ATA"
status: "wip"
protagonist: "Kia"
location: "Aakari"
length: "novel"
pitch: "To save her people from environmental devastation, Kia must free the Temple of Tef from corruption fostered by the expansionist Cult of Valor."
---

## Pitch Materials 

 ```dataview
table section, status, summary
from ""
where (story = "Temple Mage") AND (chapter = "00")  AND (status != "deleted")
sort chapter asc
```

## Chapters

 ```dataview
table chapter, location, time, summary
from ""
where (story = "Temple Mage") AND (chapter != "00")  AND (status != "deleted")
sort chapter asc
```
