## Урок 1

- Первая программа
- Ручная компиляция
- Этапы компиляции
- Байт-код
- Ветвление (if else)
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
![levels](https://user-images.githubusercontent.com/29703461/39214856-9bebdd40-481e-11e8-97fd-b68a80f43fc0.png)

### Байт-код
Чтобы отобразить байт-код класса необходимо в консоли написать (при этом вы должны находиться в папке с файлом MyFirstApp.class):
>javap -c -s -verbose название_класса

[Java байткод «Hello world»](https://habr.com/post/264919/)

### Ветвление (if else)
![turpal](https://user-images.githubusercontent.com/29703461/39215173-9afa64b4-481f-11e8-9731-fa60a8439f71.jpg)

