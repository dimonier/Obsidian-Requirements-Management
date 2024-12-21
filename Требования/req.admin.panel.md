> [!Общее]-
up:: [[Требования]]
created:: 2023-07-28
updated:: `= this.file.mday`
accociations:: 
## Анализ
requirement:: Интерфейс админки для приложения
source:: Основной заказчик
applications:: 1
type:: br
due:: 
blocks:: 
votes:: 
status:: 7-готово
## Реализация
fr:: Реализовать на фронте интерфейс админки и хранение параметров в БД на бэке
implementation:: [[us.admin]]
implemented:: 
version:: 1.0.0
tests:: 
## Критерии приёмки
ac:: Администратор видит в интерфейсе дополнительное меню "Администрирование"
ac:: Администратор может зайти в меню "Администрирование" под своим основным логином
ac:: В разделе "Администрирование" отбражаются все параметры работы приложения
ac:: Администратор может в разделе "Администрирование" видеть и изменять все отображаемые параметры
## Другие требования из этого раздела
```dataview
TABLE requirement as Требование, applications as "⚙ 👍", votes as "👤 👍", fr as "Функц. требование", implementation as "Где реализовано", status as Состояние
WHERE startswith(file.folder, this.file.folder) AND startswith(file.name, this.file.name) AND file.name != this.file.name
SORT votes DESC
```