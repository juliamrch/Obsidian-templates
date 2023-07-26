# Obsidian French Templates

Those are my templates for everyday work and side projects, self hosted on my computer with [Obsidian](https://obsidian.md).

## What kind of templates are those ?

Sometimes, I translate to French some existing templates that I find cool and create my own. Templates I reuse are in a separate folder with appropriate README and LICENCE files.

Most of the time, I create my own. You can use these models to start working with [Dataview](https://blacksmithgu.github.io/obsidian-dataview/) and create your own if you wish.

Some are business oriented, others might be more creative oriented. It really depends on the mood or if Mercury is in retrograde. For example.

### 📝 Notes

For daily and weekly logs. Includes some mecanisms to summarize and keep track, like:

- Categories from `Note Hebdo` are automatically reported to `Revue Hebdo` to create a summary.
- `daily` template includes a `dataviewjs` snippet to collect undone tasks from previous notes and to **exclude** unchecked tasks from templates (in order to avoid polluting your task feed).

⚠️ Undone tasks will be collected only from the folder where your new daily note is created. My folder is named `☀️ Morning Routine`, you can create a folder with the same name or change it on the template:

```dataviewjs
dv.header(2, '🫵 Tâches non faites');  
dv.taskList(dv.pages('"☀️ Morning Routine"').file.tasks
.where(t => !t.completed))

```

- Add `daily` as your default template for the Daily Note.

### 🚀 Projet

Templates to keep track of your projects and acomplishments. Use `Projet` as a template to write your project details. The #wip tag will add it to "Projets tech" in `tableau-de-bord`, and remove it when you change it to #done. Once you change the #wip tag to #done, your project will appear in your `🚀 Accomplissements` dashboard. 

### 💬 Réunions

These are templates for different kinds of meeting. I've connected it to my embeded calendar to create a note before a meeting.

The `suivi` doc will compile all your meeting-notes so you can easily find them.

## ⚙️ Special features?

Most templates require [DataView](https://github.com/blacksmithgu/obsidian-dataview) plugin, which you can install easiyly from the Obsidian app interface. Globally, I hightly recommend installing this very cool plugin and supporting the creator with donations.

That's it, enjoy.
