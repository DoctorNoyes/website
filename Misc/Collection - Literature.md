
## Recent  
```dataview  
TABLE  
title as Title,  
authors as "Authors",  
year as Year,  
contribution as Contribution
FROM "01 Literature Notes" OR "Readwise\Books"
SORT file.ctime desc
LIMIT 5
```

---
## Areas
#### MHSU 
```dataview
TABLE  
title as Title,  
authors as "Authors",  
year as Year,  
contribution as Contribution  
FROM "01 Literature Notes" AND #mhsu
SORT file.ctime desc
```


#### Methods

```dataview
TABLE  
title as Title,  
authors as "Authors",  
year as Year,  
contribution as Contribution  
FROM "01 Literature Notes" AND (#qualitative OR #statistics)
SORT file.ctime desc
```


## All
```dataview  
TABLE  
title as Title,  
authors as "Authors",  
year as Year,  
citekey as Citekey,  
contribution as Contribution  
FROM "01 Literature Notes"  
WHERE contains(class, "Literature")
SORT file.ctime desc
```

