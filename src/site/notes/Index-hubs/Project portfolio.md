---
{"dg-publish":true,"permalink":"/index-hubs/project-portfolio/","tags":["index-note"],"dg-note-properties":{"aliases":["project hub"],"dateCreated":"Mon, 11-05-2026, 12:02 PM","tags":["index-note"],"banner":"![System_Meta/Images/Project board.png](/img/user/System_Meta/Images/Project%20board.png)","cssclasses":["mid-view"],"banner-x":49,"banner-y":36,"emblem":"🌍","title":null}}
---

>[!navigation] Go to [[Homepage\|homepage]]
>
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
        - file.ctime.date() == today()
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
  - type: cards
    name: Paused
    filters:
      and:
        - file.ctime.date() == today()
        - status.containsAll("in-progress")
    order:
      - aliases
      - client
      - Phone-number
      - project-timeline
      - execution-team
      - progress
    columnSize:
      file.name: 451
    cardSize: 300
  - type: cards
    name: Abandoned
    filters:
      and:
        - file.ctime.date() == today()
        - status.containsAll("in-progress")
    order:
      - aliases
      - client
      - Phone-number
      - project-timeline
      - execution-team
      - progress
    columnSize:
      file.name: 451
    cardSize: 300
  - type: cards
    name: Completed
    filters:
      and:
        - file.ctime.date() == today()
        - status.containsAll("in-progress")
    order:
      - aliases
      - client
      - Phone-number
      - project-timeline
      - execution-team
      - progress
    columnSize:
      file.name: 451
    cardSize: 300
  - type: cards
    name: Closed
    filters:
      and:
        - file.ctime.date() == today()
        - status.containsAll("in-progress")
    order:
      - aliases
      - client
      - Phone-number
      - project-timeline
      - execution-team
      - progress
    columnSize:
      file.name: 451
    cardSize: 300
  - type: cards
    name: Yet-to-close
    filters:
      and:
        - file.ctime.date() == today()
        - status.containsAll("in-progress")
    order:
      - aliases
      - client
      - Phone-number
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
  - type: cards
    name: This-week
    filters:
      and:
        - file.ctime.date() < today() && file.ctime.date() >= today() - "7d"
    order:
      - aliases
      - type
      - client
      - form-entry
      - processing-fee
    sort:
      - property: project-number
        direction: DESC
    columnSize:
      file.name: 451
    cardSize: 300

```

