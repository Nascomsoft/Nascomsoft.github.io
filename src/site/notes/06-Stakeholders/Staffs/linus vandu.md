---
{"dg-publish":true,"permalink":"/06-stakeholders/staffs/linus-vandu/","tags":["people/staff"],"dg-note-properties":{"aliases":null,"dateCreated":"Mon, 18-05-2026, 12:25 PM","tags":["people/staff"],"contact-info":"[[linus vandu contact information]]","cssclasses":["mid-view"],"title":null}}
---

```base
filters:
  and:
    - file.tags.contains("task/staff")
    - '!file.name.contains("template")'
    - note["assigned-to"].contains("linus vandu")
views:
  - type: cards
    name: Todo's
    filters:
      and:
        - completed == false
        - status == "todo"
    groupBy:
      property: related-project
      direction: ASC
    order:
      - file.name
      - assigned-date
      - due-date
      - dependency
    columnSize:
      note.completed: 108
      file.name: 422
      note.status: 126
      note.assigned-date: 193
      note.due-date: 158
  - type: cards
    name: In-progress
    filters:
      and:
        - completed == false
        - status == "in-progress"
    groupBy:
      property: related-project
      direction: ASC
    order:
      - file.name
      - assigned-date
      - due-date
      - dependency
      - completed
    columnSize:
      note.completed: 108
      file.name: 422
      note.status: 126
      note.assigned-date: 193
      note.due-date: 158
  - type: cards
    name: Completed
    filters:
      and:
        - completed == true
    groupBy:
      property: related-project
      direction: ASC
    order:
      - file.name
      - assigned-date
      - due-date
      - completion-date
    columnSize:
      note.completed: 108
      file.name: 422
      note.status: 126
      note.assigned-date: 193
      note.due-date: 158
  - type: cards
    name: Closed
    filters:
      and:
        - completed == true
        - status == "closed"
    groupBy:
      property: related-project
      direction: ASC
    order:
      - file.name
      - assigned-date
      - due-date
      - completion-date
    columnSize:
      note.completed: 108
      file.name: 422
      note.status: 126
      note.assigned-date: 193
      note.due-date: 158
  - type: cards
    name: Paused
    filters:
      and:
        - status == "paused"
    groupBy:
      property: related-project
      direction: ASC
    order:
      - file.name
      - assigned-date
      - due-date
      - dependency
    columnSize:
      note.completed: 108
      file.name: 422
      note.status: 126
      note.assigned-date: 193
      note.due-date: 158
  - type: cards
    name: Abandoned
    filters:
      and:
        - status == "abandoned"
    groupBy:
      property: related-project
      direction: ASC
    order:
      - file.name
      - assigned-date
      - due-date
      - dependency
    columnSize:
      note.completed: 108
      file.name: 422
      note.status: 126
      note.assigned-date: 193
      note.due-date: 158

```







| Task                                                                   | To          |
| ---------------------------------------------------------------------- | ----------- |
| [[03-Tasks/program code for project 4\|program code for project 4]] | linus vandu |

{ .block-language-dataview}


