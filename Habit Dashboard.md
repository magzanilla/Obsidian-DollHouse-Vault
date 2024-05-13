**Habit Tracking Recent**

```dataview
TABLE choice(Habit-1, "✔", "❌") AS "Habit 1", choice(habit-2, "✔", "❌") AS "Habit 2", choice(habit-3, "✔", "❌") AS "Habit 3", choice(habit-4, "✔", "❌") AS "Habit 4"
from "Agenda"
sort file.day desc
limit 30
```



> [!NOTE] For Changing Habit Table
> It's pulling information from the daily notes in "agenda" folder.
> change the name of the habits in the [[DailyNote]] template.
> If you change the "habit-1" in the habits section to "drawing"
> 
> And the dataview below, change: 
> choice(Habit-1, "✔", "❌") AS "Habit 1"
> 
> Into (for example): 
> choice(drawing, "✔", "❌") AS "Art"
> 
> It will change the dataview header to "Art" and track the habit in daily notes named "drawing".
