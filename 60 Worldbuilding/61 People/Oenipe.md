Son of a powerful trader-lord in Nahria.  

 ```dataview
table status, location, year, length, pitch
from "80 Stories"
where protagonist = "Oenipe"
sort year desc
```

 ```dataview
table status, location, year, length, pitch
from "80 Stories"
where contains(mentions, "Oenipe")
sort year desc
```

