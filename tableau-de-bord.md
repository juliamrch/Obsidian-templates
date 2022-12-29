---
tags: ['#suivi']  
type: 'dashboard'
---

## 🛠️ Projets tech en cours
```dataview
TABLE without ID
  file.link AS "Projet",
  Description AS "💬"
  FROM #projet and #wip
```


```dataviewjs
dv.header(2, '🦄 À faire');  
dv.taskList(dv.pages('#Log/DailyLog').file.tasks
.where(t => !t.completed))

```

## À tester
```dataview
  list
  FROM #tech-test 
```


## À lire
```dataview
  list
  FROM #lire
```

   



## Idées 
```dataview
TABLE without ID Idées AS "💡", file.link as "Sources"
FROM #idées and -"Templates"
Sort file.link ascending
```
