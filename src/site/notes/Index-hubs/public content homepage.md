---
{"dg-publish":true,"permalink":"/index-hubs/public-content-homepage/","title":"🌍 Homepage","pinned":true,"tags":["note/index-hub","gardenEntry"],"dg-note-properties":{"aliases":["digital-garden-homepage"],"dateCreated":"Tue, 19-05-2026, 07:52 PM","tags":["note/index-hub","gardenEntry"],"emblem":"🌍","title":"🌍 Homepage","cssclasses":["mid-view"]}}
---

---
>[!info] Quick-Links
>- Visit the [[Index-hubs/knowledge-base hub\|knowledge base]] to find information

[[test canvas.canvas\|test canvas.canvas]]



### Assigned Tasks 
---
#### Staffs

```base
filters:
  and:
    - file.tags.contains("task/staff")
    - '!file.name.contains("template")'
views:
  - type: cards
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


---
>[!tip]- Expand the call-out to access your dedicated task page (staffs only)
>- [[Stakeholders/Staffs/linus vandu\|linus vandu]]
>- [[+Inbox/yohanna\|yohanna]]
>- [[stanley ikegbo\|stanley ikegbo]]
>- etc

---
#### Interns & volunteers

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


