---
{"dg-publish":true,"permalink":"/01-dashboards/project-management/","tags":["dashboard/home"],"ctime":"2026-06-10T22:52:09.322+01:00","mtime":"2026-10-31T15:19:59.298+01:00","dg-note-properties":{"aliases":["projects & tasks"],"dateCreated":"Mon, 11-05-2026, 12:02 PM","tags":["dashboard/home"],"banner":"[[07-System-Meta/Images/Banners/Project board.png]]","cssclasses":["full-view"],"banner-x":49,"banner-y":36,"emblem":"🌍"}}
---

- Go back to [[+Homepage\|+Homepage]]
---
[list2tab]
- Contracts
	
```base
filters:
  and:
    - file.tags.contains("project")
    - '!file.name.contains("template")'
    - state == ["contract"]
views:
  - type: cards
    name: In-progress
    filters:
      and:
        - status.containsAll("in-progress")
    order:
      - aliases
      - client
      - project-timeline
      - execution-team
      - progress
    columnSize:
      file.name: 451
    cardSize: 300

```

- Prospects
	
```base
filters:
  and:
    - file.tags.contains("project")
    - '!file.name.contains("template")'
    - state == ["prospect"]
views:
  - type: table
    name: All
    order:
      - aliases
      - state
      - client
      - form-entry
      - processing-fee
      - type
    sort:
      - property: project-number
        direction: DESC
    columnSize:
      note.aliases: 672
      note.state: 117
      note.type: 84
    cardSize: 300

```

---
### Assigned Tasks 
---
[list2tab]
- Staffs
	
```base
filters:
  and:
    - file.tags.contains("task/staff")
    - '!file.name.contains("template")'
views:
  - type: table
    name: Current Week Todo's
    filters:
      and:
        - completed == false
        - week == "W21-2026"
    groupBy:
      property: related-project
      direction: ASC
    order:
      - completed
      - file.name
      - status
      - assigned-to
      - assigned-date
      - due-date
      - completion-date
      - dependency
    sort: []
    columnSize:
      file.name: 422
      note.status: 126
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: All TODO'S
    filters:
      and:
        - completed == false
        - file.hasLink(this.file.name)
    groupBy:
      property: related-project
      direction: ASC
    order:
      - completed
      - file.name
      - status
      - assigned-to
      - assigned-date
      - due-date
      - completion-date
      - dependency
    columnSize:
      note.completed: 108
      file.name: 422
      note.status: 126
      note.assigned-date: 193
      note.due-date: 158
  - type: table
    name: In-progress
    filters:
      and:
        - status == ["in-progress"]
    groupBy:
      property: related-project
      direction: ASC
    order:
      - completed
      - file.name
      - status
      - assigned-to
      - assigned-date
      - due-date
      - completion-date
      - dependency
    columnSize:
      file.name: 422
      note.status: 126
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: Completed
    order:
      - file.name
      - due-date
      - assigned-date
      - status
      - dependency
    columnSize:
      file.name: 365
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: Paused
    filters:
      and:
        - file.hasLink(this.file.name)
    order:
      - file.name
      - due-date
      - assigned-date
      - status
      - dependency
    columnSize:
      file.name: 365
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: Abandoned
    filters:
      and:
        - file.hasLink(this.file.name)
    order:
      - file.name
      - due-date
      - assigned-date
      - status
      - dependency
    columnSize:
      file.name: 365
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: Linus Vandu
    filters:
      and:
        - completed == false
        - note["assigned-to"].contains(link("linus vandu"))
    groupBy:
      property: related-project
      direction: ASC
    order:
      - completed
      - file.name
      - status
      - due-date
      - assigned-date
      - completion-date
      - dependency
    sort: []
    columnSize:
      file.name: 422
      note.status: 126
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: Yohanna
    filters:
      and:
        - completed == false
        - note["assigned-to"].contains(link("yohanna"))
    groupBy:
      property: related-project
      direction: ASC
    order:
      - completed
      - file.name
      - status
      - due-date
      - assigned-date
      - completion-date
      - dependency
    sort: []
    columnSize:
      file.name: 422
      note.status: 126
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: Munir
    filters:
      and:
        - completed == false
        - note["assigned-to"].contains(link("yohanna"))
    groupBy:
      property: related-project
      direction: ASC
    order:
      - completed
      - file.name
      - status
      - due-date
      - assigned-date
      - completion-date
      - dependency
    sort: []
    columnSize:
      file.name: 422
      note.status: 126
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: Loveth
    filters:
      and:
        - completed == false
        - note["assigned-to"].contains(link("yohanna"))
    groupBy:
      property: related-project
      direction: ASC
    order:
      - completed
      - file.name
      - status
      - due-date
      - assigned-date
      - completion-date
      - dependency
    sort: []
    columnSize:
      file.name: 422
      note.status: 126
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: Kaseem Garba
    filters:
      and:
        - completed == false
        - note["assigned-to"].contains(link("yohanna"))
    groupBy:
      property: related-project
      direction: ASC
    order:
      - completed
      - file.name
      - status
      - due-date
      - assigned-date
      - completion-date
      - dependency
    sort: []
    columnSize:
      file.name: 422
      note.status: 126
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: Kaseem
    filters:
      and:
        - completed == false
        - note["assigned-to"].contains(link("yohanna"))
    groupBy:
      property: related-project
      direction: ASC
    order:
      - completed
      - file.name
      - status
      - due-date
      - assigned-date
      - completion-date
      - dependency
    sort: []
    columnSize:
      file.name: 422
      note.status: 126
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: CEO
    filters:
      and:
        - completed == false
        - note["assigned-to"].contains(link("yohanna"))
    groupBy:
      property: related-project
      direction: ASC
    order:
      - completed
      - file.name
      - status
      - due-date
      - assigned-date
      - completion-date
      - dependency
    sort: []
    columnSize:
      file.name: 422
      note.status: 126
      note.due-date: 158
      note.assigned-date: 193

```

- Interns & volunteers
	
```base
filters:
  and:
    - file.tags.contains("task")
    - '!file.name.contains("template")'
views:
  - type: table
    name: This Week's Tasks
    filters:
      and:
        - file.links.contains(link("linus vandu"))
    order:
      - file.name
      - related-project
      - status
      - due-date
      - assigned-date
      - dependency
    columnSize:
      file.name: 365
      note.due-date: 158
      note.assigned-date: 193
      note.status: 126
  - type: table
    name: Todo
    filters:
      and:
        - file.hasLink(this.file.name)
    order:
      - file.name
      - due-date
      - assigned-date
      - status
      - dependency
    columnSize:
      file.name: 365
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: In-progress
    filters:
      and:
        - file.hasLink(this.file.name)
    order:
      - file.name
      - due-date
      - assigned-date
      - status
      - dependency
    columnSize:
      file.name: 365
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: Completed
    filters:
      and:
        - file.hasLink(this.file.name)
    order:
      - file.name
      - due-date
      - assigned-date
      - status
      - dependency
    columnSize:
      file.name: 365
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: Paused
    filters:
      and:
        - file.hasLink(this.file.name)
    order:
      - file.name
      - due-date
      - assigned-date
      - status
      - dependency
    columnSize:
      file.name: 365
      note.due-date: 158
      note.assigned-date: 193
  - type: table
    name: Abandoned
    filters:
      and:
        - file.hasLink(this.file.name)
    order:
      - file.name
      - due-date
      - assigned-date
      - status
      - dependency
    columnSize:
      file.name: 365
      note.due-date: 158
      note.assigned-date: 193

```


