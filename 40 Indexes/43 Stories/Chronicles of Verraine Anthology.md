- [i] An anthology of short stories in the universe. Goal: 50,000 words
- [[2022.06.01 Breeder (MF)]]
- [[2021.09.01 Gregarious (MF)]]
- [[Finding Winged Island Story]]
- [[2021.12.08 Mock (MF)]]
- [[2021.07.28 Embaphium (MF)]]
- [[2022.04.27 The Apothecary's Daughter (MF)]]
- [[2021.09.08 Petrichor (MF)]]
- [[2021.12.15 Shock (MF)]]
- [[Herding Giant Spiders]]
- [[(NL) By the Blood of Mountains]]
- [[2022.03.23 Semblance (MF)]]
- [[2021.10.13 Shattered (MF)]]
- [[Marsh Runner (SS)]]
- [[Biladiyn Bred]]
- [[Biladiyn Recruitment]]
- [[Chinampa Repair Story]]
- [[2021.10.06 The laundress & the fungal growth (FF)]]
- [[2021.09.15 Vulpine (MF)]]
- [[2021.08.04 Furtive (MF)]]
- [[2021.11.03 The Impossible Knife (SS)]]
- [[2021.11.17 Contract (MF)]]
- [[2021.09.22 Effervescent (MF)]]
- [[2021.08.11 Succulent (MF)]]
- [[2021.10.20 Eavesdrop (MF)]]
- [[2022.02.02 The Bitter Business of Sweetwater Beans (FF)]]
- [[disappointed he's home]]
- [[The Dead King's Daughter]]
- [[2021.10.27 Poison (MF)]] 
- [[Hired King]]
- [[2021.09.29 Liminal (MF)]]
- [[2021.06.16 The Sea Prince (MF)]]
- [[Biladiyn Recruitment]]
- [[2022.03.02 Wyrden Eyes (SS)]] * 
- [[Pro Life]] * 
- [[Snapper Extermination]] * 
- [[2022.01.05 The Magic of Marsh Protection (FF)]]
- [[Magic Fishing]] * 
- [[Magic Sailing]] * 
- [[(MF) Smuggler]] * 

---

Where do these fit?

- [[Swordwulfen and Delia]] * 
- [[Red Rider]] * 

Wordcount:  `=sum( map(filter(this.file.inlinks, (x) => x.wordcount), (x) => sum(x.wordcount)) )`

## Attempt #3

```dataview
TABLE
    default(mentions, protagonist) AS "Characters", 
    default(time, year) AS "When",
    default(pitch, summary) AS "Overview",
    default(wordcount, length) AS "length"
FROM ""  
WHERE contains(file.inlinks, this.file.link)
```