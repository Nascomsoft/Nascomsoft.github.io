---
{"dg-publish":true,"permalink":"/06-stakeholders/staffs/linus-vandu/","tags":["people/staff"],"dg-note-properties":{"aliases":null,"dateCreated":"Mon, 18-05-2026, 12:25 PM","tags":["people/staff"],"contact-info":"[[linus vandu contact information]]","cssclasses":["mid-view"],"title":null}}
---

```base
filters:
  and:
    - file.tags.contains("task/staff")
    - '!file.name.contains("template")'
    - note["assigned-to"].contains(link("linus vandu"))
views:
  - type: cards
    name: Todo's
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

```







| Task                                                                   | To                                                                        |
| ---------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| [[03-Tasks/program code for project 4\|program code for project 4]] | <ul><li>[[06-Stakeholders/Staffs/linus vandu.md\\|linus vandu]]</li></ul> |

{ .block-language-dataview}


