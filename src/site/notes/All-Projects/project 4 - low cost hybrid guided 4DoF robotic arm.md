---
{"dg-publish":true,"permalink":"/all-projects/project-4-low-cost-hybrid-guided-4-do-f-robotic-arm/","tags":["project"],"dg-note-properties":{"dateCreated":"Wed, 13-05-2026, 07:20 PM","tags":["project"],"week":"W20-2026","emblem":"🎯","project-number":4,"aliases":["design and implementation of a low cost hybrid guided control system for a 4-DoF robotic arm"],"state":["contract"],"type":"hybrid","client":["[[Halima Ayobami Dauda]]"],"Location":"Nigeria, Bauchi state","project-scope":["construction"],"project-timeline":"2 weeks","Initial-cost(k)":100000,"form-entry":true,"processing-fee":true,"status":"in-progress","start-date":"2026-05-12","progress":["🟡🟡🟡🟡🟡🟡🟡🟡⚫⚫ 80%"],"completion-date":null,"Total-cost":"100000","execution-team":["[[Nasiru Abdulsalam|CEO]]","[[Sabui]]","[[linus vandu]]"],"rating":null,"keywords":null,"comment":null,"title":null,"cssclasses":["mid-view"]}}
---


>[!info] view project documentation

---
### Assigned tasks

>[!example] Dataview Query

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




```base
filters:
  and:
    - file.tags.contains("task")
    - '!file.name.contains("template")'
views:
  - type: table
    name: Todo's
    filters:
      and:
        - completed == false
        - file.hasLink(this.file.name)
    groupBy:
      property: due-date
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
    sort:
      - property: due-date
        direction: DESC
    columnSize:
      note.completed: 115
      file.name: 265
      note.status: 118
      note.assigned-to: 226
      note.assigned-date: 182
      note.due-date: 195
    markers: none
    kanbanViewId: 3ba4081a-a1b5-4e53-ac55-35acbfd95739
  - type: table
    name: Completed
    filters:
      and:
        - completed == true
        - file.hasLink(this.file.name)
    groupBy:
      property: assigned-date
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
    sort:
      - property: due-date
        direction: DESC
    columnSize:
      note.completed: 115
      file.name: 388
      note.status: 118
      note.assigned-to: 226
      note.assigned-date: 182
      note.due-date: 195
    markers: none
    kanbanViewId: 3ba4081a-a1b5-4e53-ac55-35acbfd95739

```

