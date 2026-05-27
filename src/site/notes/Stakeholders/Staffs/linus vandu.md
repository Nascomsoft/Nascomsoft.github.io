---
{"dg-publish":true,"permalink":"/stakeholders/staffs/linus-vandu/","tags":["people/staff"],"dg-note-properties":{"aliases":null,"dateCreated":"Mon, 18-05-2026, 12:25 PM","tags":["people/staff"],"contact-info":"[[linus vandu contact information]]]","cssclasses":["mid-view"],"title":null}}
---


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
>[!done]- Completed Tasks
>

