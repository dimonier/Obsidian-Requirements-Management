> [!Общее]-
up:: [[Требования]]
created:: 2023-07-28
updated:: `= this.file.mday`
accociations:: 
## Анализ
requirement:: Отправка уведомлений о происходящем в приложении пользователю в мессенджер
source:: Потенциальные пользователи
applications:: 
type:: ur
due:: 
blocks:: 
votes:: 2
status:: 1-новое

Подробности в [[Интеграция с мессенджерами]]
## Реализация
fr:: Должна быть возможность отправки уведомлений о происходящих событиях пользователю в мессенджер
implementation:: [[us.messages]]
implemented:: 
version:: 
tests:: 
## Другие требования из этого раздела
```dataview
TABLE requirement as Требование, applications as "⚙ 👍", votes as "👤 👍", fr as "Функц. требование", implementation as "Где реализовано", status as Состояние
WHERE startswith(file.folder, this.file.folder) AND startswith(file.name, this.file.name) AND file.name != this.file.name
SORT votes DESC
```