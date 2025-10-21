---
tags:
  - daily_note
created: <% tp.file.creation_date() %>|
estudo: false
musculacao: false
corrida/cardio: false
---
<<[[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD').subtract(1, 'd').format('YYYY-MM-DD') %>|Ontem]] | [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD').add(1, 'd').format('YYYY-MM-DD') %>|Amanhã]] >>
##### Diário
<% tp.file.cursor() %>

---------------------
##### Tarefas Feitas
```tasks
done on {{date:YYYY-MM-DD}}
hide done date
```
----------------
##### Novas tarefas
Aqui adiciono novas tarefas. 'Ctrl+L' é o atalho que ativa o plugin Tasks e ajuda a criar uma nova tarefa.