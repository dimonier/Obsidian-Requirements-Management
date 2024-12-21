> [!Общее]-
up:: [[Истории]]
created:: 2023-07-28
updated:: `= this.file.mday`
accociations:: 

## Я как `role` хочу `want` для того, чтобы `objective`
role:: пользователь системы
want:: получать сообщения об интересующих меня событиях
objective:: вовремя реагировать на события, затрагивающие мою работу
## Реализация
task:: mytask-345
parent:: [[feature.messages]]
status:: 5-бэклог
version:: 

## Дополнительно
docs:: [Прототипы интерфейса]()
docs:: [Спецификация OpenAPI]()
docs:: [Описание функциональности]()
## Реализуемые требования
```dataview
TABLE requirement as Требование, applications as "⚙ 👍", votes as "👤 👍", fr as "Функц. требование", ac as "Критерии приёмки", implementation as "Где реализовано", status as Состояние
WHERE contains(file.folder, "Управление требованиями") AND (startswith(file.name, "req.") AND (contains(implementation, this.file.name) OR contains(implementation, this.file.link)))
SORT file.name ASC
```
## Комментарии для разработки/тестирования
1. Комментарий 1
	- примечание 1
	- примечение 2
2. Комментарий 2
## Экспорт для копирования во внешнюю систему
# Описание пользовательской истории
|                 |                    |
| --------------- | ------------------ |
| Я как           | `= this.role`      |
| Хочу            | `= this.want`      |
| Для того, чтобы | `= this.objective` |

# Реализуемые требования
```dataview
TABLE requirement as Требование, applications as "⚙ 👍", votes as "👤 👍", fr as "Функц. требование", ac as "Критерии приёмки", implementation as "Где реализовано", status as Состояние
WHERE contains(file.folder, "Управление требованиями") AND (startswith(file.name, "req.") AND (contains(implementation, this.file.name) OR contains(implementation, this.file.link)))
SORT file.name ASC
```

# Связанные документы
- Задача **`= "[" + this.task + "](https://my-task-tracker/task/" + this.task + ")"`**

`= this.docs` 

![[#Комментарии для разработки/тестирования]]