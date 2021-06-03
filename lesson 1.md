> ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) — эта иконка означает, что рядом с ней находится ссылка, содержащая видеоурок: кликайте на нее для его просмотра


# ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) <a>[Занятие первое](https://drive.google.com/file/d/1l2g_mGPw3XEJ9OyURaXosRVqmeDz4kId/view?usp=sharing)</a>

## Темы занятия
1. [Подготовка рабочего окружения](#1)
1. [Первая программа](#2)
1. [Ручная компиляция и запуск программы](#3)
1. [Этапы компиляции и запуска](#4)
1. [Байт-код](#5)
1. [Переменные: примитивные типы данных](#6)
1. [Ветвление: if, if else](#7)
1. [Циклы: for, while, do while](#8)
1. [Система управления версиями Git](#9)
1. [Домашнее задание](#10)
1. [Советы по выполнению домашнего задания](#11)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 1. <a name="1">[Подготовка рабочего окружения](https://drive.google.com/file/d/1gWrBFrly3BdXKq868Xr0QkGtpM9FCmI4/view?usp=sharing)</a>
- Установите Java SE Development Kit 8:
  - для пользователей [Windows](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
  - для пользователей [Ubuntu Linux](http://help.ubuntu.ru/wiki/java)
  - альтернативная сборка [JDK 8](https://libericajdk.ru/pages/java-8u275/) для всех платформ (не требует регистрации; при установке автоматически прописыват в `PATH` путь до папки с java)
- Откройте консоль и введите в ней `java -version`, а затем `javac -version`
- Если при этом возникнет ошибка `"java/javac" не является внутренней или внешней командой, исполняемой программой или пакетным файлом`, то
  - [занесите](https://youtu.be/EEqScHr_bec) в переменную окружения `PATH` полный путь до папки, где хранятся файлы `java` и `javac`. Перезапустите консоль
- Напишите в консоли для вывода значения переменной `PATH` одну из следующих команд: 
  - `echo %PATH%` (для Windows)
  - `$PATH` (для Linux)
- Убедитесь, что в отображаемом результате присутствует путь до указанных выше файлов
- Установите систему контроля версий [Git](http://git-scm.com/downloads)
- Создайте аккаунт на [GitHub](https://github.com/)
- Для удобной навигации по файлам на GitHub установите расширение для браузера — [Octotree](https://www.octotree.io/download)
- Скачайте и установите [Sublime Text](https://www.sublimetext.com/3). Именно в нем мы будем писать наши программы (с четвертого урока перейдем на IntelliJ IDEA)
- Выполните [настройку](https://docs.google.com/document/d/1Ebi46kxKng45PLBH2dXpCnXXCHRI18rwXuDrXskWaa0/edit?usp=sharing) Sublime Text

Использовать какую-либо из IDE до четвертого урока — запрещено! Консоль, Sublime Text и "голый" Git — ваши лучшие друзья!

**Материалы:**
- [Что такое JDK? Введение в средства разработки Java](https://topjava.ru/blog/what-is-the-jdk)
- [Что такое JRE? Введение в среду выполнения Java](https://topjava.ru/blog/what-is-the-jre)
- [Что такое JVM? Знакомство с виртуальной машиной Java](https://topjava.ru/blog/what-is-the-jvm)
- [Популярность Java-технологий в 2019 году](https://topjava.ru/blog/sostoyanie-java-v-2019-godu)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 2. <a name="2">[Первая программа](https://drive.google.com/file/d/1anXQBZ80wvfzozUNlfhy1wtS-eS50cZi/view?usp=sharing)</a>

Перепишите данный код в Sublime Text:

``` java
public class MyFirstApp {	
    public static void main(String[] args) {
        System.out.println("Hello, world");
    }
}
```
и сохраните его в файле под названием `MyFirstApp.java`

**Материалы:**
- [Обзор и настройка Sublime Text](https://youtu.be/xWhTf_o86Lg)  — видео дано для ознакомления с возможностями редактора. Это не значит, что вам нужно делать все то, что делает его автор (youtube)
- [Установка плагина Terminal для SublimeText](https://youtu.be/9cFW481D2lU) (youtube)
- [Первая программа на Java – Hello World](http://pr0java.blogspot.com/2015/03/java-hello-world.html)
- ["Hello World!" Application](https://docs.oracle.com/javase/tutorial/getStarted/application/index.html)
- [Java "Hello World" Program](https://www.journaldev.com/481/java-hello-world-program)
- [Java main method](https://www.journaldev.com/12552/public-static-void-main-string-args-java-main-method)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 3. <a name="3">[Ручная компиляция и запуск программы](https://drive.google.com/file/d/1u0jyGJkFFLUwfj0c21uY2i2louNtIm_3/view?usp=sharing)</a>
Для компиляции и запуска программы необходимо в консоли перейти в папку, в которой находится файл `MyFirstApp.java`, и ввести последовательно следующие команды:
- `javac MyFirstApp.java` — компиляция java-файла
- `java MyFirstApp` — запуск программы

Для того, что бы русский текст корректно отображался в консоли, компилируйте свои программы с помощью ключа `-encoding utf8`:
- `javac -encoding utf8 имя_класса.java`

Если вы используете windows 10, то можно [настроить](https://drive.google.com/file/d/1LTDN9reLiQFdlgc8Nnx4itfMQ0hhxgkb/view?usp=sharing) ОС на поддержку Юникод. В этом случае ключ `-encoding utf8` уже не требуется.

**Материалы:**
- [Работа с командной строкой Windows](https://www.youtube.com/watch?v=8_tkUJhuogA) (youtube)
- [Введение в командную строку Windows](https://www.youtube.com/user/Iidsp/videos) (youtube)
- [Работа с Java в командной строке](https://habr.com/post/125210/)
- [Сответствие консольных команд Windows и Linux](https://white55.ru/cmd-sh.html)

## 4. <a name="4">Этапы компиляции и запуска</a>
![levels](https://user-images.githubusercontent.com/29703461/108978900-25bbb880-769b-11eb-91e9-528b66eda9c2.jpg)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 5. <a name="5">[Байт-код](https://drive.google.com/file/d/19Tl7dEpPszjQfulzQBEwyn9sQL0DK3ji/view?usp=sharing)</a>
Для отображения байт-кода класса необходимо в консоли перейти в папку, в которой находится файл `MyFirstApp.class`, и написать:
`javap -c -s -verbose MyFirstApp`

**Материалы:**
- [Java байт-код «Hello world»](https://habr.com/post/264919/)
- [javap — Disassembles one or more class files](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/javap.html)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 6. <a name="6">[Переменные: примитивные типы данных](https://drive.google.com/file/d/1mrsKC-wU7NpxQiNt47rgfySsDGTwB8Wb/view?usp=sharing)</a>

**Материалы:**
- [Переменные в Java](https://youtu.be/Y__Ns7FS5lA?t=17) (youtube)
- [Примитивные типы данных](http://developer.alexanderklimov.ru/android/java/types.php)
- [Variables](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/variables.html)
- [Primitive Data Types](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)

![var](https://user-images.githubusercontent.com/29703461/115867241-7ead9000-a443-11eb-8365-4ba0f533f7ff.png)

## Все домашние задания показывайте ментору по одному, не копите их!
- [Чек-лист](https://docs.google.com/document/d/1CcFKdXwgnL3h65izX1oY6PtUKQe9DV-I-YEQQ2RKu74/edit?usp=sharing) наиболее часто совершаемых ошибок при форматировании Java-кода. Ориентируйтесь на него при форматировании своих программ

**Домашнее задание:**
- Создайте класс **Variable** с методом **main**
- Объявите в методе переменные всех существующих в Java примитивных типов данных. Каждой переменной присвойте значение 
- В качестве значений используйте информацию о своем компьютере: количество ядер, частота процессора и тд.
- Выведите все значения переменных на консоль
- Разберитесь с [Git/GitHub](https://github.com/ichimax/startjava/blob/master/lesson%201.md#9): почитайте рекомендации о том, как с ними работать, настройте свой локальный репозиторий
- **Покажите Д/З наставнику** (пришлите ему ссылку с решенным ДЗ на ваш репозиторий на github)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 7. <a name="7">[Ветвление: if, if else](https://drive.google.com/file/d/1r-UVn4Z9OhV-SUvJdMrC6EG_v9qowAJS/view?usp=sharing)</a>
![turpal](https://user-images.githubusercontent.com/29703461/39215173-9afa64b4-481f-11e8-9731-fa60a8439f71.jpg)

**Материалы:**
- [Ветвление в Java](https://javarush.ru/groups/posts/2726-vetvlenie-v-java)
- [Оператор if else](https://youtu.be/ryR033ld_N0) (youtube)
- [The if-then and if-then-else Statements](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/if.html)

**Домашнее задание:**
- Создайте класс **ConditionalStatement** с методом **main**
- Перепишите псевдокод, приведенный ниже, с помощью Java
- Используйте переменные, условные операторы, оператор ! [(логическое НЕ)](http://developer.alexanderklimov.ru/android/java/logic_operators.php)
- Выводите сообщения на консоль
- Не используйте переменные типа String

``` java
ЕСЛИ(возраст > 20) {
    сообщение
}

ЕСЛИ(мужскойПол) {
    сообщение
}

ЕСЛИ(!мужскойПол) {
    сообщение
}

ЕСЛИ(рост < 1.80) {
    сообщение
} ИНАЧЕ {
    сообщение
}

ЕСЛИ(перваяБукваИмени == ‘M’) {
    сообщение
} ИНАЧЕ ЕСЛИ(перваяБукваИмени == ‘I’) {
    сообщение
} ИНАЧЕ {
    сообщение
} 
```
- **Покажите Д/З наставнику**

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 8. <a name="8">Циклы: [for](https://drive.google.com/file/d/1MxaPlSwY6-Nv2zOrQGYy5lOSDjYTfnfU/view?usp=sharing), [while, do while](https://drive.google.com/file/d/1YQHY9C1QbueWYFMRBpHFTqg1wt9N_333/view?usp=sharing)</a>
![loop](https://user-images.githubusercontent.com/29703461/39228479-100883f2-4867-11e8-9d63-5d18e455aaa2.jpeg)

**Материалы:**
- Циклы в Java [1](http://nikulux.ru/java-uroki/tsikly-v-yazyke-programmirovaniya-java/), [2](https://android-study.ru/урок-15-циклы-и-методы-в-java-часть-1/)
- [Оператор while](https://youtu.be/15PjODTSTaw) (youtube)
- [Оператор for](https://youtu.be/UYbdAmgcNVc) (youtube)

**Домашнее задание:**
- Создайте класс **Cycle** с методом **main**
- Выведите на консоль с помощью цикла for все числа от [0, 20]
- Выведите на консоль с помощью цикла while все числа от [6, -6] (с шагом итерации 2)
- Подсчитайте с помощью цикла do-while сумму нечетных чисел от [10, 20]. Выведите ее на консоль
- **Покажите Д/З наставнику**

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 9. <a name="9">[Система управления версиями Git](https://drive.google.com/file/d/1IMw7DA_lodW2GueWpU1nMUmYx0pnlPGA/view?usp=sharing)</a>
![image](https://cloud.githubusercontent.com/assets/18701152/15219746/9295a2fe-186d-11e6-876b-c61cc9be71e4.png)

**Материалы:**
  - [Система управления версиями](https://ru.wikipedia.org/wiki/Система_управления_версиями) (wiki)
  - [Базовый курс по обучению Git](https://www.youtube.com/playlist?list=PLIU76b8Cjem5B3sufBJ_KFTpKkMEvaTQR) (youtube)
  - [Git. Быстрый старт](https://www.youtube.com/watch?v=4-NX17Ip-xQ&list=PLmRNNqEA7JoM77hOJkPrLOfJQGizCLR3P) (youtube)
  - Интерактивные Git-обучалки: [1](https://githowto.com/ru), [2](http://learngitbranching.js.org)
  - [Официальная книга про Git](https://git-scm.com/book/ru/v2)
  
### Настройка локального репозитория
- Создайте в удобном для вас месте папку под названием `startjava`. В ней будет храниться ваш код
- Создайте на GitHub репозиторий с названием `startjava`
- Напишите в консоли (при этом консоль должна быть открыта в папке `startjava`): 
  - [`git init`](https://git-scm.com/book/ru/v1/Основы-Git-Создание-Git-репозитория#Создание-репозитория-в-существующем-каталоге) — создание локального репозитория
  - [`git status`](https://git-scm.com/book/ru/v1/Основы-Git-Запись-изменений-в-репозиторий#Определение-состояния-файлов) — вывод состояния файлов
  - добавьте адрес созданного на GitHub репозитория в git — [`git remote add origin url_на_ваш_startjava-репозиторий.git`](https://git-scm.com/book/ru/v1/Основы-Git-Работа-с-удалёнными-репозиториями)
  - проверьте, добавился он или нет — `git remote -v`

### Рекомендации по Git
1. Последовательность стандартных шагов при работе с Git:
   - [`git add файл_с_кодом.java`](https://git-scm.com/book/ru/v1/Основы-Git-Запись-изменений-в-репозиторий#Отслеживание-новых-файлов) — добавляем файлы/изменения в git (файлы с расширением class не добавляйте)
   - [`git commit -m "краткое описание изменений, которые вы внесли в программу"`](https://git-scm.com/book/ru/v1/Основы-Git-Запись-изменений-в-репозиторий#Фиксация-изменений) — фиксируем (коммитим) изменения
   - [`git push -u origin master`](https://git-scm.com/book/ru/v1/Основы-Git-Работа-с-удалёнными-репозиториями#Push) — [устанавливаем связь](https://qna.habr.com/q/118865) между локальной и удаленной веткой master
2. На GitHub отправляйте не только файлы с расширением `*.java`, но и папки, например, `Lesson 1`
3. Если вы хотите в Git добавить папку с файлами, но при этом какие-то файлы требуется проигнорировать (например `*.class`):
   - `git add "Lesson 1"`
   - `git reset "Lesson 1/имя файла, который необходимо проигнорировать"`

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 10. <a name="10">[Домашнее задание](https://drive.google.com/file/d/1Svgm_03td3Aj_MeVt-MBqSCv-PEhXD0A/view?usp=sharing)</a>

> Перед отправкой домашнего задания на проверку обращайте внимание на [`Советы по выполнению домашнего задания`](https://github.com/ichimax/startjava/blob/master/lesson%201.md#11), которые содержат ряд полезных подсказок и разъяснений
- Прочитайте первую и третью (до стр 84) главы книги [Изучаем Java](https://www.ozon.ru/context/detail/id/7821666/)
- Прочитайте первые две главы книги [Pro Git](https://git-scm.com/book/ru/v2)
- Дополнительные книги:
  - [Программирование на Java для детей, родителей, бабушек и дедушек (есть русский перевод)](http://myflex.org/books/java4kids/java4kids.htm)
  - [Яша учится программировать](https://drive.google.com/file/d/1ukTlzMrFX3Zj8X9TXp6U-mJUH1fOKUED/view?usp=sharing)
- Реализуйте `Калькулятор`, который должен уметь выполнять математические операции (`+, -, *, /, ^, %`) над целыми положительными числами:
  - что бы программа могла выполнить ту или иную математическую операцию (одну, а не все сразу), делайте проверку математического знака, используя `if else`
  - выведите на экран результат вычисления с помощью `System.out.println()`
  - Символ `^` используется в данном задании для обозначения операции возведения в степень, но в Java он выполняет совсем иную функцию. Использовать его для возведения в степень не получится. Самостоятельно реализуйте данную операцию (**не используйте Math.pow()**)
  - Символ`%`, похожий на проценты, называется [оператором деления по модулю](https://welcome4u.ru/languages/java/ostatok-ot-deleniya-v-java#i-8). В калькуляторе не надо считать проценты! Считайте остаток от деления
- Напишите игру `Угадай число`:
  - компьютер "загадывает" целое число от (0 до 100], которое необходимо угадать
  - после каждой неудачной попытки выводите подсказку:
    - `"Данное число больше того, что загадал компьютер"` или
    - `"Данное число меньше того, что загадал компьютер"`
  - если число угадано — `"Поздравляю, число угадано!"`
  - меняйте значение переменной, хранящей числа игрока, автоматически по какому-то простому алгоритму (без применения ввода с клавиатуры или генерации рандомных чисел)
  - игра продолжается до тех пор, пока число не будет угадано
- Выведите в цикле символы кодировки [Unicode](https://ru.wikipedia.org/wiki/Юникод) в диапазоне [9398, 10178]. Если выводятся кракозябры, то [33, 126]

## 11. <a name="11">Советы по выполнению домашнего задания</a>

1. Ментору ссылку на репозиторий достаточно прислать один раз (для самого первого ДЗ). Для последующих ДЗ просто сообщайте, что оно готово и можно проверять
2. Учитесь грамотно формулировать свой вопрос: "у меня не получается" может иметь тысячи причин. Пишите больше подробностей о том, что вы сделали, что конкретно не получилось, какие появляются ошибки. Присылайте в чат скрины с этими ошибками
3. При выполнении ДЗ используйте только те темы, которые изучались в текущем уроке
4. Все задания выполняйте в разных классах
5. Код пишите только **ВНУТРИ** метода `main` (для каждого класса метод `main` будет своим)
6. Ввод с клавиатуры, методы класса `Math` или `Random` пока не используйте (но, если вы знаете про них и хотите использовать — дерзайте)
7. Так должна выглядеть структура ваших папок и файлов

![tree](https://user-images.githubusercontent.com/29703461/110653920-be3f5600-81ce-11eb-9ca5-e9491a2de667.png)

## Немного мотивации
- [Shia LaBeouf Motivation for Coding](https://youtu.be/J1usv2Hn-pU)
- [Мотивация для программистов](https://www.youtube.com/watch?v=NOVaNe3jx6c)
- [Речь Стива Джобса Перед выпускниками Стенфорда](https://www.youtube.com/watch?v=WVz9E7o1mmk)
- [Мотивационный совет от Стива Джобса](https://www.youtube.com/watch?v=Z2qSUZ1o47U)
- [12 минут сильнейшей мотивации. Перелом сознания](https://www.youtube.com/watch?v=69MkvKrraC0)
