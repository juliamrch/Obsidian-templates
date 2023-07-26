
## Objectifs de la journée

1.
2.
3.

```dataviewjs
dv.header(2, '🫵 Tâches non faites');  
dv.taskList(dv.pages('"☀️ Morning Routine"').file.tasks
.where(t => !t.completed))

```

## 📍 À faire aujourd'hui

### ☎️ Appeler

- [ ] ...

### 🗑️ Paperasse

- [ ] ...

### 🕰️ Prendre rdv avec

- [x] ... ✅ 2023-07-27

## 🛠️ Je vais travailler sur...

```dataview
TABLE without ID
  file.link AS "Projet",
  Description AS "💬"
  FROM #projet-perso 
SORT file.link ASC
```


#daily