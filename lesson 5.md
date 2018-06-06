# Занятие пятое

## Темы пятого занятия
- [Введение в реляционные базы данных](#1)
- [Реляционная СУБД PostgreSQL. Терминал psql](#2)
- [Введение в SQL](#3)
- [Домашнее задание](#4)

## <a name="1">1. Введение в реляционные базы данных</a>

**Материалы:**
- [База данных](https://ru.wikipedia.org/wiki/База_данных) (wiki)
- [Реляционная база данных](https://ru.wikipedia.org/wiki/Реляционная_база_данных) (wiki)
- [Что такое базы данных, СУБД и язык SQL](https://youtu.be/GbogxIMRy-o) (youtube)
- [Основные понятия базы данных](https://youtu.be/pHjGiwhitwQ) (youtube)
- [База данных SQL](https://youtu.be/kUFDvZVETKM) (youtube)

![database2](https://user-images.githubusercontent.com/29703461/40881632-64b2d3a4-66d4-11e8-842e-366d29c783f2.png)

## <a name="2">2. Реляционная СУБД PostgreSQL. Терминал psql</a>
> Скачайте и установите [СУБД PostgreSQL](https://www.postgresql.org/download)

`sudo -u postgres psql` — запуск psql в Linux

`psql -U postgres` — запуск psql в Windows 

**Материалы:**
- [PostgreSQL](https://ru.wikipedia.org/wiki/PostgreSQL) (wiki)
- [Installation PostgreSQL || PgAdmin 4 for Windows](https://www.youtube.com/watch?v=K7pgooc2JaQ)
- [Установка и использование PostgreSQL в Ubuntu](https://www.8host.com/blog/ustanovka-i-ispolzovanie-postgresql-v-ubuntu-18-04/)
- [DB-Engines Ranking](https://db-engines.com/en/ranking)
- [PostgreSQL GUI Tools](https://wiki.postgresql.org/wiki/Community_Guide_to_PostgreSQL_GUI_Tools)
- [Документация к PostgreSQL](https://postgrespro.ru/docs/postgresql/10/index)
- [Книги по PostgreSQL](https://postgrespro.ru/education/books)
- [Интерактивный терминал PostgreSQL](https://postgrespro.ru/docs/postgresql/10/app-psql)
- [Интерактивная обучалка по PostgreSQL](https://www.pgexercises.com/) [eng]

![postgresql-10](https://user-images.githubusercontent.com/29703461/40881654-c0325af6-66d4-11e8-9a40-b7de3fb24f7b.png)

## <a name="3">3. Введение в SQL</a>

**Материалы:**
- [SQL ключи во всех подробностях](https://habr.com/company/oleg-bunin/blog/348172/)
- [Обучалка SQL](http://www.sql-ex.ru/)
- [Книга для начинающих - Изучаем SQL](https://www.ozon.ru/context/detail/id/7246798/)

## <a name="4">4. Домашнее задание</a>
- Создайте базу данных под название `Jaegers`:
  - названия столбцов: `id, modelName, mark, height, weight, status, origin, launche, kaijuKill`
  - данные о роботах брать [тут](http://pacificrim.wikia.com/wiki/Category:Jaegers)
  - занести в базу информацию о 10 роботах
- Научитесь делать следующие запросы:
  - выведите все столбцы
  - отобразите только не уничтоженных роботов
  - отобразите роботов серии Mark-5 и Mark-6
  - отсортируйте таблицу по убыванию по столбцу `mark`
  - отобразите самого старого робота
