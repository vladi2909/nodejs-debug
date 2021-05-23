# nodejs-debug

## Найденные ошибки компиляции

1 Отсутствовал PORT 4000 в app.listen. Исправлена строка 13 в файле app.js

2 Неправильно импортируется модуль. Изменил require "sequelize" на require "../db". Исправлена 2 строка в файле middleware/validate-session.js

3 Не правильный импорт Router(). Добавил require('express'). Исправлена строка 1 в файле controllers/usercontroller.js

4 Неправильный экспорт. Изменил название routers на router. Исправлена строка 116 в файле controllers/gamecontroller.js

5 Отсутствие экспорта. Добавил module.exports = sequelize. Добавлена строка 18 в файл db.js

6 Отсутствие экспорта. Добавил module.exports. Исправлена строка 1 в файле models/game.js

## Найденные ошибки логики приложения

1 Передается объект вместо параметра. Изменил req.user на req.user.id. Исправлена строка 73 в файле controllers/gamecontroller.js

2 Неправильный параметр. Изменил 'games: games' на 'games: data'. Исправлена строка 9 в файле controllers/gamecontroller.js

3 Разные имена переменных. Изменил 'passwordрash' на 'passwordHash'. Исправлена строка 11 в файле controllers/usercontroller.js

4 Body-parser передан без методов. Добавил метод json(). Исправлена строка 9 в файле app.js

5 Не связана база без указания порта: "5433". Добавил port: "5433" и переустановка 'pg' до 8 версии. Исправлены строки 6 в файле db.js и 14 в package.json