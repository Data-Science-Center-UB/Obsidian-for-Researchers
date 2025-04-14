<%*
let today = tp.date.now("YYYY-MM-DD");
let formattedToday = tp.date.now("dddd Do MMMM YYYY");
-%>

# <% formattedToday %>

# Daily Log
*Document activities, focus for today, accomplishments, or key insights.*

# Tasks
#### New
*Tasks that start today, tagged appropriately.*

#### Due Today
_Tasks with a deadline today._

**Regular Tasks:**
```tasks
due today
not done
```
**Recurring Tasks:**
```tasks
is recurring
happens on <% today %>
not done
```

#### Upcoming Tasks
_All tasks with upcoming deadlines._

```tasks
due after <% today %>
not done
```

#### Done Today
_Completed tasks for today._

```tasks
done on <% today %>
```

#### Overdue Tasks
_Tasks with deadlines before today._

```tasks
due before <% today %>
not done
```

