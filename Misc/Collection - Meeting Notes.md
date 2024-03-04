```dataview 
TABLE meeting-date as "Date", project as "Project", people as "Attendees", cal-event as "Event Link"
FROM "Misc/Meetings"
SORT file.ctime desc
```
