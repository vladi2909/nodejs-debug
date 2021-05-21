# nodejs-debug

## Найденные ошибки компиляции

1 Отсутствовал PORT 4000 в app.listen. Исправлена строка 13 в файле app.js

2 Неправильно импортируется модуль. Изменил require "sequelize" на require "../db". Исправлена 2 строка в файле middleware/validate-session.js

3 Не правильный импорт Router(). Добавил require('express'). Исправлена строка 1 в файле controllers/usercontroller.js

4 Неправильный экспорт. Изменил название routers на router. Исправлена строка 116 в файле controllers/gamecontroller.js

5 Отсутствие экспорта. Добавил module.exports = sequelize. Добавлена строка 18 в файл db.js

6 Отсутствие экспорта. Добавил module.exports. Исправлена строка 1 в файле models/game.js