Days: [[<% tp.date.yesterday("YYYY-MM-DD") %>]] <== [[<% tp.date.now("YYYY-MM-DD") %>]] ==> [[<% tp.date.tomorrow("YYYY-MM-DD") %>]]
Week: [[<% tp.date.now("YYYY") %>-W<% tp.date.now("WW") %>]] 

# Daily log











## Habits
Habit-1::
Habit-2::
Habit-3:: 
Habit-4:: 



# Tasks Due Today

```tasks
due on or before <% tp.date.now("YYYY-MM-DD") %>
not done
```


# Notes To Link

```dataview
table without id file.link as "Unlinked Notes"
from #notes and !"Templates"
where !contains(file.inlinks.file.tags, "#project")
sort file.ctime desc
```

