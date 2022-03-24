 ```dataview
table protagonist, location, length, status, pitch
from "80 Stories"
where contains(string(length), "micro") AND contains(string(universe), "Verraine")
sort status asc
```

