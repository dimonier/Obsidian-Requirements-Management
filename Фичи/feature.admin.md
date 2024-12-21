> [!Общее]-
up:: [[Фичи]]
created:: 2023-07-28
updated:: `= this.file.mday`
accociations:: 

## Use case
case:: Админка
description:: Админский интерфейс
## Реализация
task:: mytask-234
status:: 5-бэклог
version:: 
## Definition of Done
ac:: Реализован общий административный интерфейс
## Definition of Ready
- Описана логическая модель данных всех затронутых сущностей
- Описаны контракты внешних интерфейсов
- Нарисованы/обновлены диаграммы последовательностей взаимодействия между затронутыми компонентами
- Определены критерии приемки историй фичи
- Требования согласованы с командой
- Поставлены задачи на разработку и тестирование
## Реализуемые истории
```dataview
TABLE role as "Я как", want as "Хочу", objective as "Для того, чтобы", sprint as "Спринт", task as "Задача", status as Состояние, version as "Реализовано в версии"
WHERE contains(file.folder, "Управление требованиями") AND (contains(parent, this.file.name) OR contains(parent, this.file.link))
SORT file.name ASC
```

### Связанные требования
(не все, подробный список см. в реализуемых историях)
```dataview
TABLE requirement as Требование, applications as "⚙ 👍", votes as "👤 👍", fr as "Функц. требование", implementation as "Где реализовано", status as Состояние
WHERE contains(file.folder, "Управление требованиями") AND (startswith(file.name, "req.") AND (contains(file.name, replace(this.file.name, "feature.", "")) OR contains(implementation, this.file.link)))
SORT file.name ASC
```
