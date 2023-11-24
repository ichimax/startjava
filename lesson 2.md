# Занятие второе

## Разбор домашнего задания
- ![video](https://user-images.githubusercontent.com/29703461/81983788-359a6c80-9634-11ea-9b47-09a56fd3d999.png) [Калькулятор](https://drive.google.com/file/d/1VXg-RlS-DprXOjbH8s5FieOUga_PCzBZ/view?usp=sharing)
- ![video](https://user-images.githubusercontent.com/29703461/81983788-359a6c80-9634-11ea-9b47-09a56fd3d999.png) [Угадай число](https://drive.google.com/file/d/1XFSXQuUchrwD7aNsUQKjxvRtKNy1_wkx/view?usp=sharing)

**Эталонный код ДЗ 1-го урока:**
- [VariableNamesTheme](https://drive.google.com/file/d/17Fl3qSSS5l7-CdBiJAraaL5PiJAyj3gv/view?usp=sharing)
- [VariablesTheme](https://drive.google.com/file/d/1AQYnQs0G2hFx3tM8BN8v75H46I4GPNUD/view?usp=drive_link)
- [IfElseStatementTheme](https://drive.google.com/file/d/18I_TlL8f7qW45M2t_90re8JtQBn3mHDQ/view?usp=sharing)
- [CyclesTheme](https://drive.google.com/file/d/1oUH7Y-GGxVrbG7trflIPiZESxJZDyehq/view?usp=drive_link)
- [RpsGame](https://drive.google.com/file/d/14LZkJu01U1UCZWx4h2J1jdV5C5BOK9u0/view?usp=sharing)

## Темы занятия
1. [Что такое ООП](#1)
1. [Что такое класс](#2)
1. [Что такое объект](#3)
1. [Инкапсуляция: геттеры/сеттеры](#4)
1. [Ответы на вопросы](#5)
1. [Итоговые домашние задания](#6)
1. [Опросники](#7)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 1. <a name="1">[Что такое ООП](https://drive.google.com/file/d/1Jsfz5Ygb5Ct1in7MTcNV3wSsx_30D5h3/view?usp=sharing)</a>

>ООП — это одна из парадигм (методологий, способов оформления кода) программирования, основанная на принципах, предполагающих написание программного кода в виде классов и их объектов, взаимодействующих друг с другом

**Материалы:**
- ООП с примерами. Часть [1](https://habr.com/post/87119/), [2](https://habr.com/post/87205/)
- [Зачем нам ООП и что это такое](https://habr.com/post/148015/)
- [Объектно-ориентированное программирование](http://info.javarush.ru/translation/2016/01/28/Объектно-ориентированное-программирование-перевод-статьи-.html)
- [Алан Кэй, создатель ООП, про разработку, Лисп и ООП](https://habr.com/company/hexlet/blog/303754/)
- [Simula — 50 лет ООП](https://habr.com/post/345944/)

![oop](https://user-images.githubusercontent.com/29703461/39483340-b3a50496-4d7a-11e8-8e02-42a8d63de02d.jpg)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 2. <a name="2">[Что такое класс](https://drive.google.com/file/d/1AjEL8wuTK6BbiMWB2hhi_Cx6_m7NMrD1/view?usp=sharing)</a>

>Класс — это ссылочный тип данных, являющийся прототипом (blueprint, шаблоном) объекта, описывающий его характеристики и реализующий его поведение

**Материалы:**
- [Классы в Java](https://javarush.ru/groups/posts/1949-znakomstvo-s-klassami-napisanie-sobstvennihkh-klassov-konstruktorih)
- [Classes](https://docs.oracle.com/javase/tutorial/java/javaOO/classes.html)
- [What Is a Class?](https://docs.oracle.com/javase/tutorial/java/concepts/class.html)
- [Тип данных String в Java](https://habr.com/post/260767)

![class](https://user-images.githubusercontent.com/29703461/113477118-843d3900-9488-11eb-8409-728af529574d.png)

**Домашнее задание:**
- Создайте класс **Person** (без метода `main`)
- Напишите в нем поля (атрибуты), описывающие характеристики человека: `пол, имя, рост, вес, возраст`
- Проинициализируйте их какими-то значениями
- Создайте в классе методы, описывающие поведение (что он может делать) человека: `идти, сидеть, бежать, говорить, учить Java`
- В каждом методе используйте `sout` для вывода соответствующего названию метода сообщения
- Скомпилируйте класс, чтобы проверить его на ошибки (не пытайтесь его запустить, т. к. в нем нет метода `main`)
- **Для форматирования кода этого и последующих ДЗ используйте правила из [статьи](https://topjava.ru/blog/pravila-formatirovaniya-koda-v-java2)**
- **Покажите ДЗ наставнику**

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 3. <a name="3">[Что такое объект](https://drive.google.com/file/d/1hJCGeVRy-4mTTkViK219JzfLKbwLze66/view?usp=sharing)</a>

>Объект — это экземпляр какого-либо класса, обладающий характеристиками в виде полей (fields) и поведением (функционалом) в виде методов (methods)

**Материалы:**
- [What Is an Object?](https://docs.oracle.com/javase/tutorial/java/concepts/object.html)
- [Objects](https://docs.oracle.com/javase/tutorial/java/javaOO/objects.html)

![object](https://user-images.githubusercontent.com/29703461/39529416-4e58a1e6-4e2f-11e8-9a37-029871ea096a.png)

**Домашнее задание:**
- Создайте класс **Wolf**
   - объявите в нем поля: `пол, кличка, вес, возраст, окрас` (не присваивайте им значения по умолчанию)
   - реализуйте методы: `идти, сидеть, бежать, выть, охотиться`
   - в каждом методе выводите сообщение вида: `"Воет", "Сидит"` и т. д.
- Создайте класс **WolfTest** с методом **main**
  - в нем создайте объект типа **Wolf**
  - в этом же классе присвойте полям **Wolf** какие-то значения
  - получите эти значения из полей и отобразите в консоли
  - вызовите методы объекта
- **Покажите ДЗ наставнику**

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 4. <a name="4">[Инкапсуляция: геттеры/сеттеры](https://drive.google.com/file/d/1GWI8rJS6Xwbhz512R4ohdN3b0UKYnnm1/view?usp=sharing)</a>

**Материалы:**
- [Что такое инкапсуляция](https://youtu.be/nyFQvgrkoXY) (youtube)
- [Описание инкапсуляции](https://github.com/ichimax/Java-Interview-Questions/blob/master/Questions/1.%20OOP.md#Что-такое-инкапсуляция)
- [Инкапсуляция поля](https://refactoring.guru/ru/encapsulate-field) (через VPN)
- [Инкапсуляция: геттеры и сеттеры](https://youtu.be/9Uo8SYk7lbk) (youtube)
- [Геттеры и сеттеры в Java](https://topjava.ru/blog/gettery-i-settery-v-java)
- [Геттеры и сеттеры](https://javarush.ru/groups/posts/1928-getterih-i-setterih)

## 5. <a name="5"> Ответы на вопросы</a>
> в чем разница между `классом` и `объектом`? Или это одно и тоже?

Класс и объект — это разные понятия. Класс — это «чертеж», на основе которого создаются объекты. Благодаря этому «чертежу» JVM знает, какой объект ей надо создать

**Домашнее задание:**
- Модифицируйте класс **Wolf**
   - у всех полей класса пропишите модификатор `private`
   - а у его методов — `public`
   - для доступа к полям создайте геттеры и сеттеры
   - в сеттере поля `age` реализуйте проверку: если возраст волка > 8 лет, то выведите сообщение `"Некорректный возраст"`. В противном случае — сохраните значение в поле
- Модифицируйте класс **WolfTest**  
  - с помощью сеттеров присвойте полям экземпляра класса **Wolf** какие-то значения
  - считайте эти значения из полей с помощью геттеров и отобразите в консоли
- **Покажите ДЗ наставнику**

## 6. <a name="6">Итоговые домашние задания</a>
- **[Итоговые домашние задания](https://docs.google.com/document/d/1VJxMqjhRilLIqguoGvb-4T9v1jGxWQwa_KgMWEG-fmE/edit?usp=sharing)**

<details>
<summary>Так должна выглядеть структура ваших файлов и папок</summary>
 
![tree](https://github.com/ichimax/startjava/assets/29703461/4d7bf236-eedd-465f-a687-5193f6fc76fe)
</details>
 
 ## 7. <a name="7">Опросники</a>
- [Итоговый тест](https://forms.gle/F8k6FHKu85dbkGth6) позволит вам проверить, насколько хорошо вы освоили пройденные темы
- В этом небольшом [опроснике](https://forms.gle/YDyNWaaf7SssGEtAA) вы сможете поделиться своими впечатлениями (анонимно) по поводу второго урока: что (не)понравилось, как его можно улучшить и тд. Ваши ответы помогут нам доработать урок, сделав его еще лучше!
