## Урок 1

- [Первая программа](#1)
- [Ручная компиляция и запуск программы](#2)
- [Этапы компиляции и запуска](#3)
- [Байт-код](#4)
- [Ветвление (if, if else)](#5)
- [Переменные: примитивные типы данных](#6)
- [Цикл (while, for)](#7)
- [Домашнее задание](#8)


### <a name="1">1. Первая программа</a>

Напишите данный код в любом текстовом редакторе, где есть подсветка кода (например в [Sublime Text](https://www.sublimetext.com/)):

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

### <a name="2">2. Ручная компиляция и запуск программы</a>
В консоли пишем (при этом вы должны находиться в папке с файлом MyFirstApp.java):
>javac MyFirstApp.java - компиляция java-файла

>java MyFirstApp - запуск байт-кода

[Работа с Java в командной строке](https://habr.com/post/125210/)

### <a name="3">3. Этапы компиляции и запуска</a>
![levels](https://user-images.githubusercontent.com/29703461/39216711-6f3e0140-4825-11e8-89f5-3cc708ccc706.png)

### <a name="4">4. Байт-код</a>
Чтобы отобразить байт-код класса необходимо в консоли написать (при этом вы должны находиться в папке с файлом MyFirstApp.class):
>javap -c -s -verbose название_класса

[Java байт-код «Hello world»](https://habr.com/post/264919/)

### <a name="5">5. Ветвление (if, if else)</a>
![turpal](https://user-images.githubusercontent.com/29703461/39215173-9afa64b4-481f-11e8-9731-fa60a8439f71.jpg)

- [The if-then and if-then-else Statements](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/if.html)
- [Оператор if/else](http://pr0java.blogspot.ru/2015/04/ifelse.html)

### <a name="6">6. Переменные: примитивные типы данных</a>
- [Variables](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/variables.html)
- [Primitive Data Types](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)
![var](https://user-images.githubusercontent.com/29703461/39267217-debdd66c-48d4-11e8-9c88-58b2f3631840.png)

### <a name ="7">7. Цикл (while, for)</a>
![loop](https://user-images.githubusercontent.com/29703461/39228479-100883f2-4867-11e8-9d63-5d18e455aaa2.jpeg)
- [Оператор while](http://pr0java.blogspot.ru/2015/04/java-1.html)
- [Операторы for](http://pr0java.blogspot.ru/2015/04/for-foreach.html)

### <a name ="8">8. Домашнее задание</a>
- Прочитать первую главу книги [Изучаем Java](https://www.ozon.ru/context/detail/id/7821666/)
- Все задания делать в разных классах
- Реализовать в методе `main` калькулятор, который должен уметь выполнять следующие математические операции: `+, -, *, /, ^, %`
  - вывести на экран результат работы калькулятора с помощью `System.out.println()`
  - сделать так что бы калькулятор выполнился 10 раз
- Написать игру - "угадай число": компьютер загадывает число, которое вы должны угадать
  - игра продолжается до тех пор, пока число не будет угадано
- Выведите в цикле 65535 символов кодировки [Unicode](https://ru.wikipedia.org/wiki/Юникод)
