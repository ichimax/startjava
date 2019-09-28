# Занятие третье

## Разбор домашнего задания
- ![video](https://user-images.githubusercontent.com/29703461/39678117-3f25b246-518f-11e8-8be8-ca85ac4f4e29.png) [Jaeger (setters)](https://drive.google.com/file/d/1_ljcNYoajX_N48bYCRBAQOCR18telTUp/view?usp=sharing)
- ![video](https://user-images.githubusercontent.com/29703461/39678117-3f25b246-518f-11e8-8be8-ca85ac4f4e29.png) [Jaeger (constructors)](https://drive.google.com/file/d/1j-7-cA_WmlCQC_-2MgAMuQTUpKKE4ylt/view?usp=sharing)
- ![video](https://user-images.githubusercontent.com/29703461/39678117-3f25b246-518f-11e8-8be8-ca85ac4f4e29.png) [Калькулятор](https://drive.google.com/file/d/1v1MaEFTnHSpYsy4pF0a1D6kiJqQaf2he/view?usp=sharing)

## Темы третьего занятия
- [Механизм пакетов (package) в Java](#1)
- [Компиляция Java-программ. Часть II](#2)
- [.gitignore](#3)
- [Ответы на вопросы](#4)
- [Домашнее задание](#5)

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 1. <a name="1">[Механизм пакетов (package) в Java](https://drive.google.com/file/d/1dzZwKVirUys88V5_CVM0RfQ4iQcQ0cIq/view?usp=sharing)</a>
![package](https://user-images.githubusercontent.com/29703461/39955567-bd602a26-55d9-11e8-9577-f137376c4679.png)

**Материалы:**
- [Пакеты в Java](https://ru.wikipedia.org/wiki/Package_(Java)) (wiki)
-	[Зачем нужны пакеты в Java и что это такое](http://pr0java.blogspot.ru/2015/06/java.html)
-	[Пакеты](https://www.youtube.com/watch?v=a6KGNASOtK8) (youtube)
- [Правила именования пакетов](https://ru.stackoverflow.com/questions/728735/Почему-пакеты-в-java-принято-называть-в-обратную-сторону-доменного-имени)
- [Reverse domain name notation](https://en.wikipedia.org/wiki/Reverse_domain_name_notation)
- [Packages](https://docs.oracle.com/javase/tutorial/java/package/index.html)
- [Стандартные пакеты и классы Java: официальная документация](https://docs.oracle.com/javase/8/docs/api/) (eng)

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 2. <a name="2">[Компиляция Java-программ. Часть II](https://drive.google.com/file/d/13re6jwLbagQaIkmBPr3LNUc3hIEGUbiZ/view?usp=sharing)</a>
**Материалы:**
- [Работа с Java в командной строке](https://habr.com/post/125210/)
- [javac — Java programming language compiler](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/javac.html)
- [java — Launches a Java application](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/java.html)

## ![video](https://cloud.githubusercontent.com/assets/13649199/13672715/06dbc6ce-e6e7-11e5-81a9-04fbddb9e488.png) 3. <a name="3">[.gitignore](https://drive.google.com/file/d/1cJVmgrIfLo4iNDhfNkrdkkSZUKszzApN/view?usp=sharing)</a>
**Материалы:**
- [Игнорирование файлов в git](https://youtu.be/fzmCx6FLLu0)
- [Git — игнорирование файлов](https://www.youtube.com/watch?v=EjRQ8qccLCQ) (youtube)
- [Официальная документация — gitignore](https://git-scm.com/docs/gitignore)
- [Как создать файл .gitignore в Windows](https://ru.stackoverflow.com/questions/438367/Как-создать-файл-gitignore-в-windows/438370)
- [Что должно и не должно быть в .gitignore](https://ru.stackoverflow.com/questions/474556/Что-должно-и-не-должно-быть-в-gitignore-для-любого-языка-и-ide)

## 4. <a name="4">Ответы на вопросы</a>
> Как, используя класс Scanner получить тип данных char?

Например, так: `char mathOperation = reader.next().charAt(0);`

[How can I enter “char” using Scanner in java?](https://stackoverflow.com/questions/23098790/how-can-i-enter-char-using-scanner-in-java)

> Когда я компилирую, то почему-то в папке out не создается такая же структура папок, как и в папке src. При этом class-файлы появляются в корне папки out

Забыли добавить `package` в ваши классы

[Компилятор не создает папки для *.class](https://ru.stackoverflow.com/questions/451524/java-не-создает-папки-для-class)

> Я случайно занес в индекс git папку out с class-файлами. И, если я не уберу ее, то при пуше она уйдет на github. Как сделать так что бы git ее не видел и не индексировал?

Написать в консоли `git rm -r --cached out`, а после занести папку `out` в файл `.gitignore`

[Удаление файлов из индекса git'а](https://git-scm.com/book/ru/v1/Основы-Git-Запись-изменений-в-репозиторий#Удаление-файлов)

## 5. <a name="5">Домашнее задание</a>

> Перед отправкой домашнего задания на проверку обращайте внимание на [`Советы для тех, кто выполняет домашнее задание`](https://github.com/ichimax/startjava/blob/master/lesson%203.md#советы-для-тех-кто-выполняет-домашнее-задание), которые содержат ряд полезных подсказок и разъяснений
- Наведите порядок в папках и файлах в соответствии со структурой, представленной на картинке ниже
- Создайте в корне проекта (на одном уровне с папкой `src` и `out`) файл с именем `.gitignore`
- Добавьте в `.gitignore` папку с class-файлами
- Во всех классах пропишите названия пакетов
- Научитесь правильно компилировать и запускать свои программы, запустив каждую из них
- Покажите наставнику:
    - скрин консоли с компиляцией и запуском `Игры`
    - скрин с выводом дерева каталогов и файлов, начиная от папки `startjava` (для этого используйте в консоли `tree /F`)

## Советы для тех, кто выполняет домашнее задание
- Не забудьте файл `.gitignore` добавить в git (с помощью `add`)
- `-sourcepath имя_деректории` — данный ключ позволяет упростить компиляцию программы, состоящей из нескольких файлов
- После того, как вы закончите раскладывать файлы, пропишите в каждом из них пакеты, то после всех изменений вам необходимо:
  - добавить папку `src` в индекс git'а с помощью `add`
  - удалить из индекса git'а папки, которые там были ранее — `git rm -r --cached "Lesson 1" "Lesson 2"`
  - выполнить коммит
  - сделать пуш, который перезатрет текущую структуру файлов и папок на GitHub новой — `git push -f`
- Примерно так должна выглядеть структура файлов и папок как на вашем компьютере, так и на GitHub

  ![tree2](https://user-images.githubusercontent.com/29703461/40583337-508b6740-6195-11e8-8f4f-a3821bda2540.png)
