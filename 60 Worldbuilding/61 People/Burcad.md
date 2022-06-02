---
alias: Tom
---


## Appears In

```dataview
table status, location, year, length, pitch
WHERE contains(string(mentions), "Burcad") or contains(string(protagonist), "Burcad")
sort year desc
```
