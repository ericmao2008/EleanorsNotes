
## Appears In

```dataview
table status, protagonist, year, length, pitch
WHERE contains(string(mentions), "Nakayrande") or contains(string(location), "Nakayrande")
sort year desc
```
