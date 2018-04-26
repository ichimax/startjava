## Урок 1

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


### <a name="1">1. Подготовка рабочего окружения</a>
- Установите [JDK8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) (выбрать Accept License Agreement)
- Установите систему контроля версий [Git](http://git-scm.com/downloads)
- Создайте аккаунт на [GitHub](https://github.com/)
- Для удобной навигации по файлам на GitHub установите расширение для браузера - [Octotree](https://habrahabr.ru/post/223527/)
- Установите текстовый редактор с подсветкой кода, например [Sublime Text](https://www.sublimetext.com/). Именно в нем мы и будем писать наши программы

### <a name="2">2. Первая программа</a>

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

### <a name="3">3. Ручная компиляция и запуск программы</a>
В консоли пишем (при этом вы должны находиться в папке с файлом MyFirstApp.java):
>javac MyFirstApp.java — компиляция java-файла

>java MyFirstApp — запуск программы (байт-кода)

**Ресурсы:**

- [Работа с Java в командной строке](https://habr.com/post/125210/)

### <a name="4">4. Этапы компиляции и запуска</a>
![levels](https://user-images.githubusercontent.com/29703461/39216711-6f3e0140-4825-11e8-89f5-3cc708ccc706.png)

### <a name="5">5. Байт-код</a>
Чтобы отобразить байт-код класса необходимо в консоли написать (при этом вы должны находиться в папке с файлом MyFirstApp.class):
>javap -c -s -verbose название_класса

**Ресурсы:**

- [Java байт-код «Hello world»](https://habr.com/post/264919/)

### <a name="6">6. Ветвление (if, if else)</a>
![turpal](https://user-images.githubusercontent.com/29703461/39215173-9afa64b4-481f-11e8-9731-fa60a8439f71.jpg)
**Ресурсы:**

- [The if-then and if-then-else Statements](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/if.html)
- [Оператор if/else](http://pr0java.blogspot.ru/2015/04/ifelse.html)

### <a name="7">7. Переменные: примитивные типы данных</a>
**Ресурсы:**

- [Variables](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/variables.html)
- [Primitive Data Types](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)
![var](https://user-images.githubusercontent.com/29703461/39267217-debdd66c-48d4-11e8-9c88-58b2f3631840.png)

### <a name ="8">8. Цикл (while, for)</a>
![loop](https://user-images.githubusercontent.com/29703461/39228479-100883f2-4867-11e8-9d63-5d18e455aaa2.jpeg)

**Ресурсы:**

- [Оператор while](http://pr0java.blogspot.ru/2015/04/java-1.html)
- [Оператор for](http://pr0java.blogspot.ru/2015/04/for-foreach.html)

### <a name ="9">9. Система управления версиями Git</a>
![image](https://cloud.githubusercontent.com/assets/18701152/15219746/9295a2fe-186d-11e6-876b-c61cc9be71e4.png)

**Ресурсы:**

  - [Система управления версиями](https://ru.wikipedia.org/wiki/Система_управления_версиями) (wiki)
  - [Базовый курс по обучению Git](https://www.youtube.com/playlist?list=PLIU76b8Cjem5B3sufBJ_KFTpKkMEvaTQR) (youtube)
  - [Git. Быстрый старт](https://www.youtube.com/watch?v=4-NX17Ip-xQ&list=PLmRNNqEA7JoM77hOJkPrLOfJQGizCLR3P) (youtube)
  - [Официальная книга про Git](https://git-scm.com/book/ru/v2)
  - [Git обучалка](https://githowto.com/ru)
  - [Интерактивная Git обучалка (в настройках выберите русский язык)](http://learngitbranching.js.org)
  
### <a name="10">10. Настройка проекта</a>
- Создайте в удобном для вас месте папку под названием `startjava`. В ней будет храниться ваш код
- [Занесите](https://www.java.com/ru/download/help/path.xml) git в переменную окружения PATH и перезапустите консоль
- напишите в консоли (при этом консоль должна быть открыта в папке `startjava`): 
  - `git init`
  - `git status` (если ни каких ошибок не возникло, переходите к следующему пункту)
  - Создайте на GitHub репозиторий с названием `startjava`
  - `git remote add origin url_на_твой_startjava-репозиторий.git`
  - `git remote -v`

### <a name="11">11. Домашнее задание</a>
- Прочитать первую главу книги [Изучаем Java](https://www.ozon.ru/context/detail/id/7821666/)
- Прочтитать первые две главы книги [Pro Git](https://git-scm.com/book/ru/v2)
- Реализовать калькулятор, который должен уметь выполнять следующие математические операции: `+, -, *, /, ^, %`
  - вывести на экран результат работы калькулятора с помощью `System.out.println()`
- Написать игру — "угадай число": компьютер "загадывает" целое число от 0 до 100, которое вам необходимо угадать
  - после каждой неудачной опытки выводите подсказки: `System.out.println("Введенное вами число больше (меньше) того, что загадал компьютер")`
  - если число угадано — `System.out.println("Вы угадали!")`
  - игра продолжается до тех пор, пока число не будет угадано
- Выведите в цикле символы кодировки [Unicode](https://ru.wikipedia.org/wiki/Юникод) в диапазоне [9398, 10178]

### Заметки на полях
- Все задания делать в разных классах
- Код пишем только внутри метода main (для каждого класса он будет свой)
- Примерно так должна выглядеть структура ваших файлов

![tree](https://user-images.githubusercontent.com/29703461/39294598-d3a1c94e-4944-11e8-97f4-84f3bc5d2d6c.png)
- `git add перечислить_файлы,_которые_надо_занести_в_git`
- `git commit "описание изменений, которые вы сделали в программе"`
- `git push -u origin master` — это действие делайте каждый раз, когда хотите отправить свой код на github

