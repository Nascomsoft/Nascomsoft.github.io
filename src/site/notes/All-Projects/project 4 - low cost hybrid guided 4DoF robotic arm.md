---
{"dg-publish":true,"permalink":"/all-projects/project-4-low-cost-hybrid-guided-4-do-f-robotic-arm/","tags":["project"],"dg-note-properties":{"dateCreated":"Wed, 13-05-2026, 07:20 PM","tags":["project"],"week":"W20-2026","emblem":"🎯","project-number":4,"aliases":["design and implementation of a low cost hybrid guided control system for a 4-DoF robotic arm"],"state":["contract"],"type":"hybrid","client":["[[Halima Ayobami Dauda]]"],"Location":"Nigeria, Bauchi state","project-scope":["construction"],"project-timeline":"2 weeks","Initial-cost(k)":100000,"form-entry":true,"processing-fee":true,"status":"in-progress","start-date":"2026-05-12","progress":["🟡🟡🟡🟡🟡🟡🟡🟡⚫⚫ 80%"],"completion-date":null,"Total-cost":"100000","execution-team":["[[Nasiru Abdulsalam|CEO]]","[[Sabui]]","[[linus vandu]]"],"rating":null,"keywords":null,"comment":null,"title":null,"cssclasses":["mid-view"]}}
---


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


----




