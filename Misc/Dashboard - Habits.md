
### Last 7 Days
```dataview
TABLE WITHOUT ID
  file.link as Date,
  choice(exercise = true, "✅", "・") as Exercise,
  choice(article = true, "✅", "・") as Articles,
  choice(meditation = true, "✅", "・") as Meditate,
  choice(read = true, "✅", "・") as Reading,
  choice(write = true, "✅", "・") as Writing
FROM "00 Journal/001 Daily"
WHERE file.day <= date(now) AND file.day >= date(now) - dur(7days)
SORT file.day DESC
```

### Last 30 Days 
```dataview
TABLE WITHOUT ID
  file.link as Date,
  choice(exercise = true, "✅", "・") as Exercise,
  choice(article = true, "✅", "・") as Articles,
  choice(meditation = true, "✅", "・") as Meditate,
  choice(read = true, "✅", "・") as Reading,
  choice(write = true, "✅", "・") as Writing
FROM "00 Journal/001 Daily"
WHERE file.day <= date(now) AND file.day >= date(now) - dur(30days)
SORT file.day DESC
```
