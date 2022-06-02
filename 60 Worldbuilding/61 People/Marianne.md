
## Appears In

```dataview
table status, location, year, length, pitch
WHERE contains(string(mentions), "Marianne") or contains(string(protagonist), "Marianne") or contains(protagonist, "Marianne")
sort year desc
```
