
## To Do

```dataview
TABLE tags as "Tags"
WHERE contains(class, "Card") AND contains(status, "To Do")
SORT file.mtime
```

## In-Progress

```dataview
TABLE tags as "Tags"
WHERE contains(class, "Card") AND contains(status, "In Progress")
SORT file.mtime
```

## Done

```dataview
TABLE tags as "Tags"
WHERE contains(class, "Card") AND contains(status, "Done")
SORT file.mtime
```



```dataview
TABLE tags as "Tags"
WHERE contains(class, "Card") AND contains(status, "To Do")
SORT file.mtime
```
