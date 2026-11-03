---
{"dg-publish":true,"permalink":"/00-dashboards/project-and-tasks-management-dashboard/","title":"✅️ Task Assignment","tags":["dashboard"],"dg-note-properties":{"aliases":["project and tasks dashboard"],"dateCreated":"Sat, 31-10-2026, 03:02 PM","tags":["dashboard"],"banner":"[[03-Vault/Images/Banners/Project board.png]]","cssclasses":["full-view"],"banner-x":49,"banner-y":36,"emblem":"🌍","title":"✅️ Task Assignment"}}
---

>[!Example] 🎯 All Active Projects
>
>```dataview
>TABLE WITHOUT ID
> file.link AS "Project",
>choice(
> (date(today) - date(started)).days < 7,
>   (date(today) - date(started)).days + " days",
>   choice(
>      (date(today) - date(started)).days < 30,
>      round((date(today) - date(started)).days / 7, 1) + " weeks",
>      round((date(today) - date(started)).days / 30, 1) + " months"
>    )
>  ) AS "Time Active"
>FROM #project AND #in-progress
>WHERE started
>SORT started ASC

---
- For complain about any tasks you were assigned, find information you need [[here]]
- For information regarding the project you were assigned, view [[project info]] or go directly to the [[public drive]] and download what you need

### Overdue / Not Completed

>[!Failure]  NO OVERDUE TASKS

----
### In-progress

>[!tip] Week 45
>- 
>- 
>- 

----
### Completed

>[!success]- TO BE UPDATED
>- 
>  
