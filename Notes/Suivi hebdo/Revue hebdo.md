

---
created: ["{{date}} {{time}}"]
tags: ["#Log/WeeklyLog"]
---
___


# 🔎 Synthèse

```dataview
TABLE WITHOUT ID
	link(file.name) as "Semaine",
	tech AS "⚙️",
	priorité AS "📍",
	bof AS "☹️",
	cool AS "✌️",
	idée AS "💡"
WHERE file.folder = this.file.folder AND
 contains(tag, "#WeeklyNote")
SORT file.name ASC
```

## Clients débloqués de la semaine

```dataview
TABLE without ID
  Qui AS "👤",
  Quoi AS "Quoi",
  Comment AS "Comment",
  file.link as "Quand"
FROM #débloqué and -"Templates"
WHERE file.folder = this.file.folder AND
 contains(tag, "#WeeklyNote")
Sort file.link ascending
```



## Divers

### 🤔 Questions
```dataview
LIST question
WHERE file.folder = this.file.folder AND
 contains(tag, "#WeeklyNote")
```

### 🤓 Remarques
```dataview
LIST remarque
WHERE file.folder = this.file.folder AND
 contains(tag, "#WeeklyNote")
```
