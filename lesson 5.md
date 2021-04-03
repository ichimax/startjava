# Занятие пятое

## Темы пятого занятия
- [Введение в реляционные базы данных](#1)
- [Реляционная СУБД PostgreSQL. Терминал psql](#2)
- [Введение в SQL](#3)
- [Домашнее задание](#4)
- [Советы по выполнению домашнего задания](#5)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) <a name="1">1. [Введение в реляционные базы данных](https://drive.google.com/file/d/16JpQcAwKyhFQkh0D6et2RMVXx2fUFBkc/view?usp=sharing)</a>

**Материалы:**
- [База данных](https://ru.wikipedia.org/wiki/База_данных) (wiki)
- [Реляционная база данных](https://ru.wikipedia.org/wiki/Реляционная_база_данных) (wiki)
- [Что такое базы данных, СУБД и язык SQL](https://youtu.be/GbogxIMRy-o) (youtube)
- [Основные понятия базы данных](https://youtu.be/pHjGiwhitwQ) (youtube)
- [База данных SQL](https://youtu.be/kUFDvZVETKM) (youtube)

![database2](https://user-images.githubusercontent.com/29703461/40881632-64b2d3a4-66d4-11e8-842e-366d29c783f2.png)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) <a name="2">2. [Реляционная СУБД PostgreSQL. Терминал psql](https://drive.google.com/file/d/1GQulzZEjzfvbOVcK7rXagprbpkMm0rg5/view?usp=sharing)</a>
> Скачайте и установите [СУБД PostgreSQL](https://www.postgresql.org/download)

`sudo -u postgres psql` — запуск psql в Linux

`psql -U postgres` — запуск psql в Windows 

**Материалы:**
- [PostgreSQL](https://ru.wikipedia.org/wiki/PostgreSQL) (wiki)
- [Installation PostgreSQL || PgAdmin 4 for Windows](https://www.youtube.com/watch?v=e1MwsT5FJRQ)
- [Установка и использование PostgreSQL в Ubuntu](https://www.8host.com/blog/ustanovka-i-ispolzovanie-postgresql-v-ubuntu-18-04/)
- [DB-Engines Ranking](https://db-engines.com/en/ranking)
- [PostgreSQL GUI Tools](https://wiki.postgresql.org/wiki/Community_Guide_to_PostgreSQL_GUI_Tools)
- [Документация к PostgreSQL](https://postgrespro.ru/docs/postgresql/10/index)
- [Книги по PostgreSQL](https://postgrespro.ru/education/books)
- [Интерактивный терминал PostgreSQL](https://postgrespro.ru/docs/postgresql/10/app-psql)
- [Интерактивная обучалка по PostgreSQL](https://www.pgexercises.com/) [eng]

![postgresql-10](https://user-images.githubusercontent.com/29703461/40881654-c0325af6-66d4-11e8-9a40-b7de3fb24f7b.png)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) <a name="3">3. [Введение в SQL](https://drive.google.com/file/d/1NTxcqFXVFgEHcQGNhX8GkchXgdvFs-g3/view?usp=sharing)</a>

**Материалы:**
- [SQL ключи во всех подробностях](https://habr.com/company/oleg-bunin/blog/348172/)
- [Обучалка SQL](http://www.sql-ex.ru/)
- [Книга для начинающих - Изучаем SQL](https://www.ozon.ru/context/detail/id/7246798/)

## <a name="4">4. Домашнее задание</a>

> Перед отправкой домашнего задания на проверку обращайте внимание на [`Советы по выполнению домашнего задания`](#5), которые содержат ряд полезных подсказок и разъяснений
- Создайте базу данных и таблицу под название `Jaegers`:  
  - названия столбцов: `id, modelName, mark, height, weight, status, origin, launch, kaijuKill`
  - SQL-код размещайте в файле `create_db.sql`
- Заполните таблицу данными:     
  - занесите информацию о 10 роботах (если каких-то данных будет не хватать — придумайте их самостоятельно)
  - данные о роботах берите [тут](http://pacificrim.wikia.com/wiki/Category:Jaegers)
  - SQL-код размещайте в файле `init_db.sql`
- Научитесь делать следующие запросы:
  - выведите всю таблицу
  - отобразите только не уничтоженных роботов
  - отобразите роботов нескольких серий, например Mark-1 и Mark-6
  - отсортируйте таблицу по убыванию по столбцу `mark`
  - отобразите самого старого робота
  - отобразите роботов, которые уничтожили больше/меньше всех kaiju
  - отобразите средний вес роботов
  - увеличьте на единицу количество уничтоженных kaiju у роботов, которые до сих пор не разрушены
  - удалите уничтоженных роботов
  - SQL-код размещайте в файле `queries.sql`
- Запуште созданные и заполненные SQL-файлы на GitHub и покажите наставнику
- Найдите в справке к [psql](https://postgrespro.ru/docs/postgresql/13/app-psql) ключ, который позволит вам запустить данные файлы из консоли
- Пришлите наставнику скриншоты консоли с запущенным файлом `queries.sql`

## <a name="5">5. Советы по выполнению домашнего задания</a>
- Если при запуске SQL-файла возникает ошибка `Permission denied`, выполните [эти](https://dba.stackexchange.com/questions/29767/permission-denied-in-file-trying-to-import) рекомендации
- Если при работе с psql некорректно отображается кодировка, выполните [эти](https://iu5bmstu.ru/index.php?title=PostgreSQL_-_%D0%9A%D0%B8%D1%80%D0%B8%D0%BB%D0%BB%D0%B8%D1%86%D0%B0_%D0%B2_psql_%D0%BF%D0%BE%D0%B4_Windows) настройки
- Так должна выглядеть структура ваших папок и файлов

![tree2](https://user-images.githubusercontent.com/29703461/112764796-deff0c80-9012-11eb-980f-eb4869e12268.png)
