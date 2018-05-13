# Занятие третье

## Темы третьего занятия
- [Механизм пакетов (package) в Java](#1)
- [Компиляция Java-программ по-взрослому](#2)
- [.gitignore](#3)
- [Ответы на вопросы](#4)
- [Домашнее задание](#5)

## 1. <a name="1">Механизм пакетов (package) в Java</a>
![package](https://user-images.githubusercontent.com/29703461/39955567-bd602a26-55d9-11e8-9577-f137376c4679.png)

**Материалы:**
- [Пакеты в Java](https://ru.wikipedia.org/wiki/Package_(Java)) (wiki)
-	[Зачем нужны пакеты в Java и что это такое](http://pr0java.blogspot.ru/2015/06/java.html)
-	[Пакеты](https://www.youtube.com/watch?v=a6KGNASOtK8) (youtube)
- [Правила именования пакетов](https://ru.stackoverflow.com/questions/728735/Почему-пакеты-в-java-принято-называть-в-обратную-сторону-доменного-имени)
- [Reverse domain name notation](https://en.wikipedia.org/wiki/Reverse_domain_name_notation)
- [Packages](https://docs.oracle.com/javase/tutorial/java/package/index.html)
- [Стандартные пакеты и классы Java: официальная документация](https://docs.oracle.com/javase/8/docs/api/) (eng)


## 2. <a name="2">Компиляция Java-программ. Часть II</a>
**Материалы:**
- [Исполнение классов в пакетах и CLASSPATH](http://pr0java.blogspot.ru/2015/06/java.html)
- [Работа с Java в командной строке](https://habr.com/post/125210/)
- [javac — Java programming language compiler](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/javac.html)
- [java — Launches a Java application](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/java.html)

## 3. <a name="3">.gitignore</a>
**Материалы:**
- [Игнорирование файлов в git](https://youtu.be/fzmCx6FLLu0)
- [Git — игнорирование файлов](https://www.youtube.com/watch?v=EjRQ8qccLCQ) (youtube)
- [Официальная документация — gitignore](https://git-scm.com/docs/gitignore)
- [Как создать файл .gitignore в Windows](https://ru.stackoverflow.com/questions/438367/Как-создать-файл-gitignore-в-windows/438370)
- [Что должно и не должно быть в .gitignore](https://ru.stackoverflow.com/questions/474556/Что-должно-и-не-должно-быть-в-gitignore-для-любого-языка-и-ide)

## 3. <a name="4">Ответы на вопросы</a>
> Как, используя класс Scanner получить тип данных char?

Например, так: `char mathOperation = reader.next().charAt(0);`

[How can I enter “char” using Scanner in java?](https://stackoverflow.com/questions/23098790/how-can-i-enter-char-using-scanner-in-java)

> Когда я компилирую, то почему-то в папке out не создается такая же структура папок, как и в папке src. При этом class-файлы появляются в корне папки out

[Компилятор не создает папки для *.class](https://ru.stackoverflow.com/questions/451524/java-не-создает-папки-для-class)

> Я случайно занес в индекс git папку out с class-файлами. И, если я не уберу ее, то при пуше она уйдет на github. Как сделать так что бы git ее не видел и не индексировал?

написать в консоли `git -rm -r --cached out`, а после занести папку `out` в файл `.gitignore`



## 4. <a name="5">Домашнее задание</a>
- Наведите порядок в папках с файлами (относится ко всем выполненным ранее урокам)
- Создайте в корне проекта (на одном уровне с папкой `src` и `out`) файл с именем `.gitignore`
- Добавьте в `.gitignore` папку с class-файлами
- Научитесь правильно компилировать и запускать свои программы

## Заметки на полях
- Примерно так должна выглядеть структура ваших файлов

  ![tree2](https://user-images.githubusercontent.com/29703461/39961096-ade5540a-5637-11e8-9300-0336b88da8fd.png)
