## Урок 1

- Первая программа
- Ручная компиляция
- Этапы компиляции
- Байт-код
- Ветвление (if, if else)
- Переменные: примитивные типы данных
- Цикл (while, for)
- Дописать HW1


### Первая программа

Пишите код в любом текстовом редакторе, где есть подсветка кода (например в Sublime Text):

``` java
public class MyFirstApp {
	
	public static void main(String[] args) {
		System.out.println("Hello, world");
	}
}
```
**Ресурсы:**
- ["Hello World!" Application](https://docs.oracle.com/javase/tutorial/getStarted/application/index.html)
- [Java "Hello World" Program](https://www.journaldev.com/481/java-hello-world-program)
- [Java main method](https://www.journaldev.com/12552/public-static-void-main-string-args-java-main-method)

### Ручная компиляция
В консоли пишем (при этом вы должны находиться в папке с файлом MyFirstApp.java):
>javac MyFirstApp.java

>java MyFirstApp

[Работа с Java в командной строке](https://habr.com/post/125210/)

### Этапы компиляции
![levels](https://user-images.githubusercontent.com/29703461/39216711-6f3e0140-4825-11e8-89f5-3cc708ccc706.png)

### Байт-код
Чтобы отобразить байт-код класса необходимо в консоли написать (при этом вы должны находиться в папке с файлом MyFirstApp.class):
>javap -c -s -verbose название_класса

[Java байткод «Hello world»](https://habr.com/post/264919/)

### Ветвление (if, if else)
![turpal](https://user-images.githubusercontent.com/29703461/39215173-9afa64b4-481f-11e8-9731-fa60a8439f71.jpg)

- [The if-then and if-then-else Statements](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/if.html)
- [Оператор if/else](http://pr0java.blogspot.ru/2015/04/ifelse.html)

### Переменные: примитивные типы данных
- [Variables](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/variables.html)
- [Primitive Data Types](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)
![var](https://user-images.githubusercontent.com/29703461/39217299-0f919ce0-4828-11e8-81a4-f15bfa34ef68.jpg)

### Цикл (while, for)
- [Оператор while](http://pr0java.blogspot.ru/2015/04/java-1.html)
- [Операторы for](http://pr0java.blogspot.ru/2015/04/for-foreach.html)

### Домашнее задание
- Реализовать две дополнительные математические операции: возведение в степень и остаток от деления
- Написать игру - угадай число
- Исправить код калькулятора, используя переменные
- Сделать так что бы калькулятор выполнился 10 раз
