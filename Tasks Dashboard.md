
**Task Calendar**
```dataviewjs
await dv.view("tasksCalendar", {pages: "", view: "month", firstDayOfWeek: "1", options: "style7"})
```



> [!NOTE] Credit
> Tasks calendar is from [Obsidian Tasks Calendar](https://github.com/702573N/Obsidian-Tasks-Calendar/blob/main/tasksCalendar/view.css) on Github
> And in this vault is intended to get tasks from daily notes and the like.
> The Task calendar is dependent on the files in the Media Files / tasksCalendar sub-folder. As long as view.js and view.css is in the vault, it will work.

## All Unfinished Tasks

```dataview
TASK
FROM "Agenda/1. Daily"
WHERE !completed
```

> Note: can click on the task's text and go to what note file its in

## Tasks Success Chart

![[TaskChart]]

> Automatically updates