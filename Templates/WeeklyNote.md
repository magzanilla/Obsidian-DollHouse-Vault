---
tag: weekly
---

**Note Created**: {{date:LL}} {{time:LT}}

> [!NOTE] Notice
> The weeks start on Monday


## Navigation
**Weeks**:  [[<% tp.date.now("YYYY") %>-W<% tp.date.now("WW") %>]] | [[<% tp.date.now("YYYY") %>-W<% tp.date.now("WW") - -2 %>]] 

**Daily Notes**:
- **Monday** [[<% tp.date.weekday("YYYY-MM-DD", 1) %>]]
- **Tuesday** [[ <% tp.date.weekday("YYYY-MM-DD", 2) %>]]
- **Wednesday** [[<% tp.date.weekday("YYYY-MM-DD", 3) %>]]
 - **Thursday** [[<% tp.date.weekday("YYYY-MM-DD", 4) %>]]
- **Friday** [[<% tp.date.weekday("YYYY-MM-DD", 5) %>]]
- **Saturday** [[<% tp.date.weekday("YYYY-MM-DD", 6) %>]]
- **Sunday** [[<% tp.date.weekday("YYYY-MM-DD", 7) %>]]

## Week's Summary
> Talk about the week's highlights and summary here.

## Incomplete Tasks For The Week

**Unfinished tasks due before sunday**:
```tasks
due on or before <% tp.date.weekday("YYYY-MM-DD", 7) %>
not done
```

or 

**Unfinished task due between Monday and Sunday**:

```tasks
due on or after <% tp.date.weekday("YYYY-MM-DD", 1) %>
due on or before 
not done
```

or Unfinished Tasks scheduled before Sunday:

```tasks
scheduled on or before <% tp.date.weekday("YYYY-MM-DD", 7) %>
not done
```

Choose whichever want to see.