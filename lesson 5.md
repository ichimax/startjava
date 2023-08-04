# Занятие пятое

**Эталонный код ДЗ 4-го урока:**
- [ArraysTheme](https://drive.google.com/file/d/1eGOIp7FJ2e-hCxyzLofI0XvDfIj-f7xP/view?usp=sharing)
- [CalculatorTest](https://drive.google.com/file/d/1KUHnC5k5e3Jv0cQeXUyLHbNPGgxB6qwT/view?usp=sharing), [Calculator](https://drive.google.com/file/d/1AoLJlPgtJFsh3-NjylTCjxfVWacroPof/view?usp=sharing)
- [CalculatorTest*](https://drive.google.com/file/d/1uUHVlfNdkfAl9LdG9Bd_ff0XtLNIGL2L/view?usp=sharing), [Calculator*](https://drive.google.com/file/d/1tbRorYRoYLovekaHerV6yh8dGR8FFTY7/view?usp=sharing)
- [GuessNumberTest](https://drive.google.com/file/d/19i1GZWPFCGQqXYMBg5dlWBefHRw_dtdT/view?usp=sharing), [Player](https://drive.google.com/file/d/13FrnxhgBWjSdpUCTeZ3aZ6H8SNoITtWD/view?usp=sharing), [GuessNumber](https://drive.google.com/file/d/1-3rNgJTKj-5S5wlfi7FJW2fPE2sYw8Yh/view?usp=sharing)
- [GuessNumberTest*](https://drive.google.com/file/d/15cMQHqp8_Ljy6Cz6TyC6Vn5XVGhjeU-6/view?usp=sharing), [Player*](https://drive.google.com/file/d/1iO5-CCU2uE3x1RbjgukpyPvPn0s8y2Vz/view?usp=sharing), [GuessNumber*](https://drive.google.com/file/d/1pEEyzwzMlIT_BTenB6ESCtUN3-wkzZ9H/view?usp=sharing)
- Выпускной: [BookshelfTest](https://drive.google.com/file/d/1z12bzUUJVVR-64CgsWUcXEGkIrQ8zA3u/view?usp=sharing), [Book](https://drive.google.com/file/d/1qIIZgCG0GL0QTxBPGmv4cIjuikofLpX3/view?usp=sharing), [Bookshelf](https://drive.google.com/file/d/1k2JdlQjcSMozEvCKNrXMfbkweL1ZLJ7b/view?usp=sharing)

## Темы пятого занятия
1. [Введение в реляционные базы данных](#1)
1. [Реляционная СУБД PostgreSQL. Терминал psql](#2)
1. [Введение в SQL](#3)
1. [Домашнее задание](#4)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) <a name="1">1. [Введение в реляционные базы данных](https://drive.google.com/file/d/16JpQcAwKyhFQkh0D6et2RMVXx2fUFBkc/view?usp=sharing)</a>

**Материалы:**
- [Что такое базы данных, СУБД и язык SQL](https://youtu.be/GbogxIMRy-o) (youtube)
- [Основные понятия базы данных](https://youtu.be/pHjGiwhitwQ) (youtube)
- [База данных SQL](https://youtu.be/kUFDvZVETKM) (youtube)

![database2](https://user-images.githubusercontent.com/29703461/40881632-64b2d3a4-66d4-11e8-842e-366d29c783f2.png)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) <a name="2">2. [Реляционная СУБД PostgreSQL. Терминал psql](https://drive.google.com/file/d/1GQulzZEjzfvbOVcK7rXagprbpkMm0rg5/view?usp=sharing)</a>
Скачайте и установите [СУБД PostgreSQL](https://www.postgresql.org/download)

- `psql -U postgres` — запуск `psql` в Windows
- `sudo -u postgres psql` — запуск `psql` в Linux

> - Для запуска `psql` из консоли необходимо [занести](https://bestprogrammer.ru/baza-dannyh/podklyuchitsya-k-komandnoj-stroke-bazy-dannyh-postgresql-windows) в переменную `PATH` путь до папки `bin`
> - При подключении к базе данных потребуется ввести пороль, ввод которого [не будет отображаться](https://stackru.com/questions/847564/psql-nevozmozhno-vvesti-parol)

**Материалы:**
- [Установка и настройка PostgreSQL в Windows](https://youtu.be/aLDMDR8FKuk) (youtube)
- [Установка и настройка PostgreSQL в Ubuntu](https://youtu.be/n4sNHdnXj6Q) (youtube)
- [Документация к PostgreSQL](https://postgrespro.ru/docs/postgresql/15/index)
- [Документация к psql](https://postgrespro.ru/docs/postgresql/15/app-psql) 
- [DB-Engines Ranking](https://db-engines.com/en/ranking)
- [PostgreSQL GUI Tools](https://wiki.postgresql.org/wiki/Community_Guide_to_PostgreSQL_GUI_Tools)
- [Книги по PostgreSQL](https://postgrespro.ru/education/books)

![postgresql-10](https://user-images.githubusercontent.com/29703461/40881654-c0325af6-66d4-11e8-9a40-b7de3fb24f7b.png)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) <a name="3">3. [Введение в SQL](https://drive.google.com/file/d/1NTxcqFXVFgEHcQGNhX8GkchXgdvFs-g3/view?usp=sharing)</a>

**Материалы:**
- [SQL ключи во всех подробностях](https://habr.com/company/oleg-bunin/blog/348172/)
- [Обучалка SQL](http://www.sql-ex.ru/)
- [SQL для простых смертных](https://ozon.ru/t/9oR10jk)
- [Интерактивный тренажер по SQL](https://stepik.org/course/63054/promo)
- [Интерактивная обучалка по PostgreSQL](https://www.pgexercises.com/)
- [Руководство по стилю SQL](https://www.sqlstyle.guide/ru/)

## <a name="4">4. Домашнее задание</a>
- [**Домашнее задание**](https://docs.google.com/document/d/1f7JXmsZ0ZF7ECw814GzgG7BcpEDZvhbO8vBbWbiab3w/edit?usp=sharing)
- Так должна выглядеть структура ваших папок и файлов

![tree2](https://user-images.githubusercontent.com/29703461/169653431-2077ee1a-1d57-4c60-95cf-47e5701febd4.png)
