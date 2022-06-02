Urban fantasy. 

```dataview
table year, length, status, protagonist, location, pitch
from ""
where contains(universe, "Neith") and status != "deleted"
SORT number(year) ASC
```