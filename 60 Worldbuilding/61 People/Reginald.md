
## Appears In

```dataview
table status, location, time, length, pitch
WHERE contains(string(mentions), "Reginald") or contains(string(protagonist), "Reginald")
sort year desc
```