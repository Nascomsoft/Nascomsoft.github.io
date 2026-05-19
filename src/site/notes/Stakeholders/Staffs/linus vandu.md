---
{"dg-publish":true,"permalink":"/stakeholders/staffs/linus-vandu/","tags":["staff"],"dg-note-properties":{"aliases":null,"dateCreated":"Mon, 18-05-2026, 12:25 PM","tags":["staff"],"cssclasses":["mid-view"],"title":null}}
---


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


---
>[!done]- Completed Tasks
>

