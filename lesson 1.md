# Занятие первое

## Темы первого занятия
- [Подготовка рабочего окружения](#1)
- [Первая программа](#2)
- [Ручная компиляция и запуск программы](#3)
- [Этапы компиляции и запуска](#4)
- [Байт-код](#5)
- [Ветвление (if, if else)](#6)
- [Переменные: примитивные типы данных](#7)
- [Цикл (while, for)](#8)
- [Система управления версиями Git](#9)
- [Настройка локального репозитория](#10)
- [Домашнее задание](#11)

## 1. <a name="1">Подготовка рабочего окружения</a>
- Установите [Java SE Development Kit 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
- Установите систему контроля версий [Git](http://git-scm.com/downloads)
- Создайте аккаунт на [GitHub](https://github.com/)
- Для удобной навигации по файлам на GitHub установите расширение для браузера — [Octotree](https://habr.com/post/223527/)
- Установите текстовый редактор с подсветкой кода, например [Sublime Text](https://www.sublimetext.com/3). Именно в нем мы будем писать наши программы
- **Использовать какую-либо из IDE — запрещено! Консоль, Sublime Text и "голый" git — ваши лучшие друзья!**

## 2. <a name="2">Первая программа</a>

Введите данный код в Sublime Text:

``` java
public class MyFirstApp {	
	public static void main(String[] args) {
		System.out.println("Hello, world");
	}
}
```
и сохраните его в файле под названием `MyFirstApp.java`

**Материалы:**
- [Обзор и настройка Sublime Text](https://xakep.ru/2014/07/28/sublime-text-not-for-coding/)
- [SublimeText - Terminal Access - Plugin](https://www.youtube.com/watch?v=4hZvb8sr1cE) (youtube)
- [Первая программа на Java – Hello World](http://pr0java.blogspot.com/2015/03/java-hello-world.html)
- ["Hello World!" Application](https://docs.oracle.com/javase/tutorial/getStarted/application/index.html)
- [Java "Hello World" Program](https://www.journaldev.com/481/java-hello-world-program)
- [Java main method](https://www.journaldev.com/12552/public-static-void-main-string-args-java-main-method)

## 3. <a name="3">Ручная компиляция и запуск программы</a>
- Откройте консоль и введите в ней `java -version`
- Если при этом возникнет ошибка
![error](https://user-images.githubusercontent.com/29703461/39296698-4796325e-494a-11e8-8ac5-53cf4b3c3e6d.jpg),то
- [Занесите](https://www.java.com/ru/download/help/path.xml) в переменную окружения `PATH` полный путь до папки, где хранятся файлы `java` и `javac`. Перезапустите консоль
- Выведите в консоли значение переменной `PATH`: 
  - `echo %PATH%` (в win)
  - `$PATH` (в Linux)
- Убедитесь, что там присутствует путь до указанных выше файлов

Для компиляции и запуска программы необходимо в консоли перейти в папку, в которой находится файл `MyFirstApp.java`, и ввести последовательно следующие команды:
- `javac MyFirstApp.java` — компиляция java-файла

- `java MyFirstApp` — запуск программы

**Материалы:**
- [Работа с командной строкой Windows](https://www.youtube.com/watch?v=8_tkUJhuogA) (youtube)
- [Введение в командную строку Windows](https://www.youtube.com/user/Iidsp/videos) (youtube)
- [Работа с Java в командной строке](https://habr.com/post/125210/)

## 4. <a name="4">Этапы компиляции и запуска</a>
![levels](https://user-images.githubusercontent.com/29703461/39407954-5ff88c7c-4bd7-11e8-96d6-1456d6673a45.png)

## 5. <a name="5">Байт-код</a>
Для отображения байт-кода класса необходимо в консоли перейти в папку, в которой находится файл `MyFirstApp.class`, и написать:
- `javap -c -s -verbose MyFirstApp`

**Материалы:**
- [Java байт-код «Hello world»](https://habr.com/post/264919/)
- [javap — Disassembles one or more class files](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/javap.html)

## 6. <a name="6">Ветвление (if, if else)</a>
![turpal](https://user-images.githubusercontent.com/29703461/39215173-9afa64b4-481f-11e8-9731-fa60a8439f71.jpg)

**Материалы:**
- [Ветвление в Java](https://vertex-academy.com/tutorials/ru/vetvlenie-v-java/)
- [Оператор if else](http://pr0java.blogspot.ru/2015/04/ifelse.html)
- [The if-then and if-then-else Statements](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/if.html)

## 7. <a name="7">Переменные: примитивные типы данных</a>

**Материалы:**
- [Переменные в Java](https://vertex-academy.com/tutorials/ru/sozdanie-peremennyx-i-tipy-peremenny/)
- [Примитивные типы данных](http://developer.alexanderklimov.ru/android/java/types.php)
- [Variables](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/variables.html)
- [Primitive Data Types](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)

![var](https://user-images.githubusercontent.com/29703461/39386134-d0843ce6-4a7b-11e8-8a0f-94224b256386.png)

## 8. <a name ="8">Цикл (while, for)</a>
![loop](https://user-images.githubusercontent.com/29703461/39228479-100883f2-4867-11e8-9d63-5d18e455aaa2.jpeg)

**Материалы:**
- [Циклы в Java](https://vertex-academy.com/tutorials/ru/cikly-v-java/)
- [Оператор while](http://pr0java.blogspot.ru/2015/04/while.html)
- [Оператор for](http://pr0java.blogspot.ru/2015/04/for-foreach.html)

## 9. <a name ="9">Система управления версиями Git</a>
![image](https://cloud.githubusercontent.com/assets/18701152/15219746/9295a2fe-186d-11e6-876b-c61cc9be71e4.png)

**Материалы:**
  - [Система управления версиями](https://ru.wikipedia.org/wiki/Система_управления_версиями) (wiki)
  - [Базовый курс по обучению Git](https://www.youtube.com/playlist?list=PLIU76b8Cjem5B3sufBJ_KFTpKkMEvaTQR) (youtube)
  - [Git. Быстрый старт](https://www.youtube.com/watch?v=4-NX17Ip-xQ&list=PLmRNNqEA7JoM77hOJkPrLOfJQGizCLR3P) (youtube)
  - [Официальная книга про Git](https://git-scm.com/book/ru/v2)
  - [Git обучалка](https://githowto.com/ru)
  - [Интерактивная Git обучалка (в настройках выберите русский язык)](http://learngitbranching.js.org)
  
## 10. <a name="10">Настройка локального репозитория</a>
- Создайте в удобном для вас месте папку под названием `startjava`. В ней будет храниться ваш код
- Создайте на GitHub репозиторий с названием `startjava`
- Напишите в консоли (при этом консоль должна быть открыта в папке `startjava`): 
  - [`git init`](https://git-scm.com/book/ru/v1/Основы-Git-Создание-Git-репозитория#Создание-репозитория-в-существующем-каталоге)
  - [`git status`](https://git-scm.com/book/ru/v1/Основы-Git-Запись-изменений-в-репозиторий#Определение-состояния-файлов)
  - добавьте адрес созданного репозитория в git — [`git remote add origin url_на_ваш_startjava-репозиторий.git`](https://git-scm.com/book/ru/v1/Основы-Git-Работа-с-удалёнными-репозиториями)
  - проверьте, добавился он или нет — `git remote -v`

## 11. <a name="11">Домашнее задание</a>
- Прочитайте первую и третью (до стр 84) главы книги [Изучаем Java](https://www.ozon.ru/context/detail/id/7821666/)
- Прочитайте первые две главы книги [Pro Git](https://git-scm.com/book/ru/v2)
- Реализуйте `Калькулятор`, который должен уметь выполнять математические операции (`+, -, *, /, ^, %`) над целыми положительными числами:
  - для проверки знака математической операции воспользуйтесь оператором `if else`
  - выведите на экран результат работы калькулятора с помощью `System.out.println()`
- Напишите игру `Угадай число`:
  - компьютер "загадывает" целое число от 0 до 100, которое вам необходимо угадать
  - после каждой неудачной попытки выводите подсказки: `System.out.println("Введенное вами число больше (меньше) того, что загадал компьютер")`
  - если число угадано — `System.out.println("Вы угадали!")`
  - игра продолжается до тех пор, пока число не будет угадано
- Выведите в цикле символы кодировки [Unicode](https://ru.wikipedia.org/wiki/Юникод) в диапазоне [9398, 10178]. Если выводятся кракозябры, то [33, 126]

## Советы для тех, кто выполняет домашнее задание
1. Учитесь грамотно формулировать свой вопрос: "у меня не работает" может иметь тысячи причин
2. Выполните ДЗ, используя только те темы, которые изучаются в данном уроке
3. Все задания выполняйте в разных классах
4. Код пишите только **ВНУТРИ** метода `main` (для каждого класса метод `main` будет своим)
5. Ввод с клавиатуры и методы класса `Math` или `Random` пока не используйте
6. Последовательность стандартных шагов при работе с git:
   - [`git add Файл_с_кодом.java`](https://git-scm.com/book/ru/v1/Основы-Git-Запись-изменений-в-репозиторий#Отслеживание-новых-файлов) (файлы с расширением class не заносите)
   - [`git commit -m "описание изменений, которые вы внесли в программу"`](https://git-scm.com/book/ru/v1/Основы-Git-Запись-изменений-в-репозиторий#Фиксация-изменений)
   - [`git push -u origin master`](https://git-scm.com/book/ru/v1/Основы-Git-Работа-с-удалёнными-репозиториями#Push)
7. На GitHub отправляйте не только файлы с расширением Java, но и папки, например, `Lesson 1`
8. Символ `^` используется для обозначения операции возведения в степень
9. Примерно так должна выглядеть структура ваших файлов и папок

![tree](https://user-images.githubusercontent.com/29703461/40510917-c8e835ce-5fa6-11e8-9450-36ec4b878410.png)

## Немного мотивации
- [Shia LaBeouf Motivation for Coding](https://youtu.be/J1usv2Hn-pU)
- [Мотивация для программистов](https://www.youtube.com/watch?v=NOVaNe3jx6c)
- [Речь Стива Джобса Перед выпускниками Стенфорда](https://www.youtube.com/watch?v=WVz9E7o1mmk)
- [Мотивационный совет от Стива Джобса](https://www.youtube.com/watch?v=Z2qSUZ1o47U)
- [12 минут сильнейшей мотивации. Перелом сознания](https://www.youtube.com/watch?v=69MkvKrraC0)
