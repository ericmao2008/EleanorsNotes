
## Appears In

```dataview
table status, location, year, time, length, pitch
WHERE contains(string(mentions), "<% tp.file.title %>") or contains(string(protagonist), "<% tp.file.title %>")
sort year desc
```