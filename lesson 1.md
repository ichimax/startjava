# Занятие первое

- [Подготовка рабочего окружения](#1)
- [Первая программа](#2)
- [Ручная компиляция и запуск программы](#3)
- [Этапы компиляции и запуска](#4)
- [Байт-код](#5)
- [Ветвление (if, if else)](#6)
- [Переменные: примитивные типы данных](#7)
- [Цикл (while, for)](#8)
- [Система управления версиями Git](#9)
- [Настройка проекта](#10)
- [Домашнее задание](#11)

## <a name="1">1. Подготовка рабочего окружения</a>
- Установите [JDK8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) (выбрать Accept License Agreement)
- Установите систему контроля версий [Git](http://git-scm.com/downloads)
- Создайте аккаунт на [GitHub](https://github.com/)
- Для удобной навигации по файлам на GitHub установите расширение для браузера - [Octotree](https://habrahabr.ru/post/223527/)
- Установите текстовый редактор с подсветкой кода, например [Sublime Text](https://www.sublimetext.com/). Именно в нем мы и будем писать наши программы
- **Использовать какую-либо из IDE — запрещено! Консоль, Sublime Text и "голый" git — ваши лучшие друзья!**

## <a name="2">2. Первая программа</a>

Напишите данный код:

``` java
public class MyFirstApp {	
	public static void main(String[] args) {
		System.out.println("Hello, world");
	}
}
```
**Ресурсы:**
- [Обзор и настройка Sublime Text](https://xakep.ru/2014/07/28/sublime-text-not-for-coding/)
- [SublimeText - Terminal Access - Plugin](https://www.youtube.com/watch?v=4hZvb8sr1cE)
- ["Hello World!" Application](https://docs.oracle.com/javase/tutorial/getStarted/application/index.html)
- [Java "Hello World" Program](https://www.journaldev.com/481/java-hello-world-program)
- [Java main method](https://www.journaldev.com/12552/public-static-void-main-string-args-java-main-method)

## <a name="3">3. Ручная компиляция и запуск программы</a>
Для компиляции и запуска программы из предыдущего пункта (да и для всех остальных) необходимо в консоли написать (при этом консоль должна быть открыта в папке с файлом `MyFirstApp.java`):
>javac MyFirstApp.java — компиляция java-файла

>java MyFirstApp — запуск программы (байт-кода)

**Ресурсы:**
- [Работа с командной строкой Windows](https://www.youtube.com/watch?v=8_tkUJhuogA) (youtube)
- [Работа с Java в командной строке](https://habr.com/post/125210/)
- [javac — Java programming language compiler](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/javac.html)
- [java — Launches a Java application](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/java.html)

## <a name="4">4. Этапы компиляции и запуска</a>
![levels](https://user-images.githubusercontent.com/29703461/39407954-5ff88c7c-4bd7-11e8-96d6-1456d6673a45.png)

## <a name="5">5. Байт-код</a>
Чтобы отобразить байт-код класса, необходимо в консоли написать (при этом консоль должна быть открыта в папке с файлом `MyFirstApp.class`):
>javap -c -s -verbose MyFirstApp

**Ресурсы:**

- [Java байт-код «Hello world»](https://habr.com/post/264919/)
- [javap — Disassembles one or more class files](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/javap.html)

## <a name="6">6. Ветвление (if, if else)</a>
![turpal](https://user-images.githubusercontent.com/29703461/39215173-9afa64b4-481f-11e8-9731-fa60a8439f71.jpg)
**Ресурсы:**

- [The if-then and if-then-else Statements](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/if.html)
- [Оператор if/else](http://pr0java.blogspot.ru/2015/04/ifelse.html)

## <a name="7">7. Переменные: примитивные типы данных</a>
**Ресурсы:**

- [Variables](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/variables.html)
- [Primitive Data Types](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)

![var](https://user-images.githubusercontent.com/29703461/39386134-d0843ce6-4a7b-11e8-8a0f-94224b256386.png)

## <a name ="8">8. Цикл (while, for)</a>
![loop](https://user-images.githubusercontent.com/29703461/39228479-100883f2-4867-11e8-9d63-5d18e455aaa2.jpeg)

**Ресурсы:**

- [Оператор while](http://pr0java.blogspot.ru/2015/04/java-1.html)
- [Оператор for](http://pr0java.blogspot.ru/2015/04/for-foreach.html)

## <a name ="9">9. Система управления версиями Git</a>
![image](https://cloud.githubusercontent.com/assets/18701152/15219746/9295a2fe-186d-11e6-876b-c61cc9be71e4.png)

**Ресурсы:**

  - [Система управления версиями](https://ru.wikipedia.org/wiki/Система_управления_версиями) (wiki)
  - [Базовый курс по обучению Git](https://www.youtube.com/playlist?list=PLIU76b8Cjem5B3sufBJ_KFTpKkMEvaTQR) (youtube)
  - [Git. Быстрый старт](https://www.youtube.com/watch?v=4-NX17Ip-xQ&list=PLmRNNqEA7JoM77hOJkPrLOfJQGizCLR3P) (youtube)
  - [Официальная книга про Git](https://git-scm.com/book/ru/v2)
  - [Git обучалка](https://githowto.com/ru)
  - [Интерактивная Git обучалка (в настройках выберите русский язык)](http://learngitbranching.js.org)
  
## <a name="10">10. Настройка проекта</a>
- Создайте в удобном для вас месте папку под названием `startjava`. В ней будет храниться ваш код
- Откройте консоль и введите в ней `java -version`
- Если при этом возникнет ошибка
![error](https://user-images.githubusercontent.com/29703461/39296698-4796325e-494a-11e8-8ac5-53cf4b3c3e6d.jpg),то
- [Занесите](https://www.java.com/ru/download/help/path.xml) в переменную окружения `PATH` полный путь до папки, где хранятся файлы `java`, `javac`, `javap` и перезапустите консоль
- Напишите в консоли (при этом консоль должна быть открыта в папке `startjava`): 
  - `git init`
  - `git status` (внимательно читаем, что вывела команда. Если ни каких ошибок не возникло, переходите к следующему пункту)
  - Создайте на GitHub репозиторий с названием `startjava`
  - `git remote add origin url_на_твой_startjava-репозиторий.git` — добавьте, созданный вами репозиторий в git
  - `git remote -v` — посмотрите, добавился он или нет

## <a name="11">11. Домашнее задание</a>
- Прочитайте первую и третью (до стр 84) главы книги [Изучаем Java](https://www.ozon.ru/context/detail/id/7821666/)
- Прочитайте первые две главы книги [Pro Git](https://git-scm.com/book/ru/v2)
- Реализуйте калькулятор, который должен уметь выполнять следующие математические операции над целыми положительными числами: `+, -, *, /, ^, %`
  - выведите на экран результат работы калькулятора с помощью `System.out.println()`
- Напишите игру — "угадай число": компьютер "загадывает" целое число от 0 до 100, которое вам необходимо угадать
  - после каждой неудачной опытки выводите подсказки: `System.out.println("Введенное вами число больше (меньше) того, что загадал компьютер")`
  - если число угадано — `System.out.println("Вы угадали!")`
  - игра продолжается до тех пор, пока число не будет угадано
- Выведите в цикле символы кодировки [Unicode](https://ru.wikipedia.org/wiki/Юникод) в диапазоне [9398, 10178]

## Заметки на полях
1. Учитесь грамотно формулировать свой вопрос: «у меня не работает» может иметь тысячи причин
2. Все задания делать в разных классах
3. Код пишем только **ВНУТРИ** метода `main` (для каждого класса метод `main` будет своим)
4. Примерно так должна выглядеть структура ваших файлов
![tree](https://user-images.githubusercontent.com/29703461/39294598-d3a1c94e-4944-11e8-97f4-84f3bc5d2d6c.png)
5. `echo %PATH%` (на win) или `$PATH` (на Linux) — отображение значения переменной PATH
6. `git add Файл_с_кодом.java` (файлы с расширением class не заносить) — добавьте файлы в git
7. `git commit -m "описание изменений, которые вы внесли в программу"` — зафиксируйте изменения кода в git
8. `git push -u origin master` — это действие делайте каждый раз, когда хотите отправить свой код на github

## Немного мотивации
- [Shia LaBeouf Motivation for Coding](https://youtu.be/J1usv2Hn-pU)
- [Мотивация для программистов](https://www.youtube.com/watch?v=NOVaNe3jx6c)
- [Речь Стива Джобса Перед выпускниками Стенфорда](https://www.youtube.com/watch?v=WVz9E7o1mmk)
- [Мотивационный совет от Стива Джобса](https://www.youtube.com/watch?v=Z2qSUZ1o47U)
- [12 минут сильнейшей мотивации. Перелом сознания](https://www.youtube.com/watch?v=69MkvKrraC0)
