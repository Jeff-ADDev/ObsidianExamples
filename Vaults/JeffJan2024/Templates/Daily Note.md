---
date: <% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "YYYY-MM-DD") %>
week: <% tp.date.now("YYYY-[W]W", 0, tp.file.title, "YYYY-MM-DD") %>
year: <% tp.date.now("YYYY", 0, tp.file.title, "YYYY-MM-DD") %>
tags:
  - dailies
---
## <% moment(tp.file.title, "YYYY-MM-DD").format("dddd Do MMMM YYYY") %>
<< [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD').subtract(1, 'd').format('YYYY-MM-DD') %>|Yesterday]] | [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD').add(1, 'd').format('YYYY-MM-DD') %>|Tomorrow]] >>

-----
### Workout Plan



------
- > [!warning]+ [[Action Dashboard| OverDue ]]
> ```tasks
> not done
> sort by due date
> due before <% tp.date.now("YYYY-MM-DD") %>
> ((path includes 2023/03 Daily) OR (path includes 2023/02 Weekly)) AND NOT (path includes Books To Read) 
> hide backlink
> limit 10
> ```

- > [!todo]+ Today and Future Tasks
> ```tasks
> not done
> (due <% tp.date.now("YYYY-MM-DD") %>) OR (due after <% tp.date.now("YYYY-MM-DD") %>)
> ((path includes 2023/03 Daily) OR (path includes 2023/02 Weekly)) AND NOT (path includes Books To Read) 
> sort by path
> sort by priority
> hide backlink
> limit 10
> ```

- > [!todo]+ Unscheduled Tasks  
 > ```tasks  
 > not done  
 > ((path includes 2023/03 Daily) OR (path includes 2023/02 Weekly)) AND NOT (path includes Books To Read) 
> no due date
> sort by priority  
> hide backlink

- > [!success]+ Tasks Done Today
> ```tasks 
> done <% tp.date.now("YYYY-MM-DD") %>
> ((path includes 2023/03 Daily) OR (path includes 2023/02 Weekly)) AND NOT (path includes Books To Read) 
>  hide due date
>  hide backlink

------
#### New Tasks


-----
### Habits
> [!success]+ Health
> [Sleep:: ]
> [Exercise:: ]
> [Reading:: ]
> [Meditation:: ]
> [Writing:: ]


-----
### Daily Review


