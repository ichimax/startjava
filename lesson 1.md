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
1. [Опросники](#11)
1. [Советы по выполнению домашнего задания](#12)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 1. <a name="1">[Подготовка рабочего окружения](https://drive.google.com/file/d/1gWrBFrly3BdXKq868Xr0QkGtpM9FCmI4/view?usp=sharing)</a>

- [Установите и настройте Java](https://topjava.ru/blog/ustanovka-i-nastroyka-java)
- Скачайте и установите [Sublime Text 4](https://www.sublimetext.com/download). Именно в нем мы будем писать наши программы (с четвертого урока перейдем на IntelliJ IDEA)

**[Отключите](https://chromefaq.ru/nastrojki/kak-perevodit-stranitsy-v-google-chrome-s-anglijskogo-na-russkij#i-6) в браузере автоперевод страниц. Из-за него уроки могут отображаться некорректно.**

**Материалы:**
- [Что такое JDK? Введение в средства разработки Java](https://topjava.ru/blog/what-is-the-jdk)
- [Что такое JRE? Введение в среду выполнения Java](https://topjava.ru/blog/what-is-the-jre)
- [Что такое JVM? Знакомство с виртуальной машиной Java](https://topjava.ru/blog/what-is-the-jvm)
- Отчет о популярности Java-технологий в [2019](https://topjava.ru/blog/sostoyanie-java-v-2019-godu), в 2021 ([1](https://drive.google.com/file/d/1hoTlpu0Lxi0zaMZKuzDQnx287vxUlDdk/view?usp=sharing), [2](https://drive.google.com/file/d/1hLK5_qr1QoSLoPv785V3TXA1CFkkebV3/view?usp=sharing), [3](https://www.jetbrains.com/lp/devecosystem-2021/java))

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 2. <a name="2">[Первая программа](https://drive.google.com/file/d/1anXQBZ80wvfzozUNlfhy1wtS-eS50cZi/view?usp=sharing)</a>

- Изучите статью [Java с нуля: первая программа](https://topjava.ru/blog/pervaya-programma-na-java). В ней показано создание простой программы MyFirstApp с main-методом, а также дается подробный разбор каждой строки кода:

``` java
public class MyFirstApp {	
    public static void main(String[] args) {
        System.out.println("Write once, run anywhere");
    }
}
```

- [Настройте](https://topjava.ru/blog/nastroyka-sublime-text-dlya-java) Sublime Text для Java

**Материалы:**
- [Обзор и настройка Sublime Text](https://youtu.be/xWhTf_o86Lg) — видео дано для ознакомления с возможностями редактора. Это не значит, что вам нужно делать все то, что делает его автор (youtube)
- [Установка плагина Terminal для SublimeText](https://youtu.be/9cFW481D2lU) (youtube) — можно использовать либо этот плагин, либо `Terminus`

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 3. <a name="3">[Ручная компиляция и запуск программы](https://drive.google.com/file/d/1u0jyGJkFFLUwfj0c21uY2i2louNtIm_3/view?usp=sharing)</a>
Для компиляции и запуска программы необходимо в консоли перейти в папку, в которой находится файл `MyFirstApp.java`, и ввести последовательно следующие команды:
- `javac MyFirstApp.java` — компиляция java-файла
- `java MyFirstApp` — запуск программы

Для того, чтобы русский текст корректно отображался в консоли, компилируйте свои программы с помощью специального параметра `javac -encoding utf8 имя_класса.java`

Более подробно об этом рассказывается в статье [Компиляция и запуск Java-программ](https://topjava.ru/blog/kompilyatsiya-i-zapusk-programm-na-java).

А из статьи ["Основы командной строки для Java-программиста"](https://topjava.ru/blog/osnovy-komandnoy-stroki-dlya-java-programmista) вы узнаете о самых нужных и часто используемых командах консоли для работы с файловой системой 

**Материалы:**
- [Getting Started with Java](https://dev.java/learn/getting-started-with-java/)
- [Введение в командную строку Windows](https://www.youtube.com/user/Iidsp/videos) (youtube)

## 4. <a name="4">Этапы компиляции и запуска</a>
![levels](https://user-images.githubusercontent.com/29703461/108978900-25bbb880-769b-11eb-91e9-528b66eda9c2.jpg)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 5. <a name="5">[Байт-код](https://drive.google.com/file/d/19Tl7dEpPszjQfulzQBEwyn9sQL0DK3ji/view?usp=sharing)</a>
Для отображения байт-кода класса необходимо в консоли перейти в папку, в которой находится файл `MyFirstApp.class`, и написать:
`javap -c -s -verbose MyFirstApp`

**Материалы:**
- [Java байт-код «Hello world»](https://habr.com/post/264919/)
- [javap — Disassembles one or more class files](https://docs.oracle.com/en/java/javase/17/docs/specs/man/javap.html)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 6. <a name="6">[Переменные: примитивные типы данных](https://drive.google.com/file/d/1mrsKC-wU7NpxQiNt47rgfySsDGTwB8Wb/view?usp=sharing)</a>

**Материалы:**
- [Переменные в Java](https://youtu.be/Y__Ns7FS5lA?t=17) (youtube)
- [Примитивные типы данных](http://developer.alexanderklimov.ru/android/java/types.php)
- [Variables](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/variables.html)
- [Primitive Data Types](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html)

![var](https://user-images.githubusercontent.com/29703461/155842985-5fae137b-3967-4fe6-893c-0d2a018815a5.png)

- **[Домашние задания по теме "Переменные: примитивные типы данных"](https://docs.google.com/document/d/1kJqeCC-fKWUjBjrmHJ1mjDu45SGRL39Q5vW4DmLJflA/edit?usp=sharing)**
- [Изучите статью](https://topjava.ru/blog/pravila-formatirovaniya-koda-v-java) про форматирование кода в Java. Ориентируйтесь на разбираемые в ней правила при написании своих программ
- Разберитесь с [Git/GitHub](https://github.com/ichimax/startjava/blob/master/lesson%201.md#9): почитайте рекомендации о том, как с ними работать, настройте свой локальный репозиторий
- **Покажите ДЗ наставнику** (пришлите ему ссылку с решенными ДЗ на ваш репозиторий)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 7. <a name="7">[Ветвление: if, if else](https://drive.google.com/file/d/1r-UVn4Z9OhV-SUvJdMrC6EG_v9qowAJS/view?usp=sharing)</a>

**Материалы:**
- [Ветвление в Java](https://javarush.ru/groups/posts/2726-vetvlenie-v-java)
- [Оператор if else](https://youtu.be/ryR033ld_N0) (youtube)
- [The if-then and if-then-else Statements](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/if.html)

![turpal](https://user-images.githubusercontent.com/29703461/39215173-9afa64b4-481f-11e8-9731-fa60a8439f71.jpg)

- **[Домашние задания по теме "Ветвление: if-else"](https://docs.google.com/document/d/1LZLCupFXrCmTuaT4KCUW9nKjrzaFDCCH7i5PDpWSLjI/edit?usp=sharing)**
- **Покажите ДЗ наставнику**

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 8. <a name="8">Циклы: [for](https://drive.google.com/file/d/1MxaPlSwY6-Nv2zOrQGYy5lOSDjYTfnfU/view?usp=sharing), [while, do while](https://drive.google.com/file/d/1YQHY9C1QbueWYFMRBpHFTqg1wt9N_333/view?usp=sharing)</a>
![loop](https://user-images.githubusercontent.com/29703461/39228479-100883f2-4867-11e8-9d63-5d18e455aaa2.jpeg)

**Материалы:**
- Циклы в Java [1](http://nikulux.ru/java-uroki/tsikly-v-yazyke-programmirovaniya-java/), [2](https://vertex-academy.com/tutorials/ru/cikly-v-java/)
- [Оператор while](https://youtu.be/15PjODTSTaw) (youtube)
- [Оператор for](https://youtu.be/UYbdAmgcNVc) (youtube)

**Домашнее задание:**
- **[Домашние задания по теме "Циклы: for, while, do while"](https://docs.google.com/document/d/1lHSSOzARTx6tfD-4MV-t41S5bnvdNw5hczkQPT05png/edit?usp=sharing)**
- **Покажите ДЗ наставнику**

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 9. <a name="9">[Система управления версиями Git](https://drive.google.com/file/d/1IMw7DA_lodW2GueWpU1nMUmYx0pnlPGA/view?usp=sharing)</a>
![image](https://user-images.githubusercontent.com/29703461/154850409-7a618576-1105-48a1-9e32-88a34e87693b.png)

- [Установите и настройте Git/GitHub](https://topjava.ru/blog/vvedeniye-v-git-github-ustanovka-i-nastroyka)

**Материалы:**
  - [Система управления версиями](https://ru.wikipedia.org/wiki/Система_управления_версиями) (wiki)
  - [Базовый курс по обучению Git](https://www.youtube.com/playlist?list=PLIU76b8Cjem5B3sufBJ_KFTpKkMEvaTQR) (youtube)
  - [Git. Быстрый старт](https://www.youtube.com/watch?v=4-NX17Ip-xQ&list=PLmRNNqEA7JoM77hOJkPrLOfJQGizCLR3P) (youtube)
  - Интерактивные Git-обучалки: [1](https://githowto.com/ru), [2](http://learngitbranching.js.org)
  - [Официальная книга про Git](https://git-scm.com/book/ru/v2)
  
### Настройка локального репозитория
Более подробно об этом рассказывается в статье [Введение в Git/GitHub: базовые команды](https://topjava.ru/blog/vvedeniye-v-git-github-bazovyye-komandy).

- Создайте в удобном для вас месте папку под названием `StartJava`. В ней будет храниться ваш код
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
- [Программирование на Java для детей, родителей, бабушек и дедушек (есть русский перевод)](http://myflex.org/books/java4kids/java4kids.htm)
- [Итоговые домашние задания](https://docs.google.com/document/d/1m6y5qBMfwKjm0DIo3JYqQ9_QNyhroDvsRAirEyDEP7s/edit?usp=sharing)

## 11. <a name="11">Опросники</a>
- [Итоговый тест](https://forms.gle/YFc2pf6qZw6jdfXM7) позволит вам проверить, насколько хорошо вы осовили пройденные в уроке темы
- В этом небольшом [опроснике](https://forms.gle/dsthsvh1tRhdJyhu9) вы сможете поделиться своими впечатлениями (анонимно) по поводу первого урока: что (не)понравилось, как его можно улучшить и тд. Ваши ответы помогут нам доработать урок, сделав его еще лучше!

## 12. <a name="12">Советы по выполнению домашнего задания</a>

1. Ментору ссылку на репозиторий достаточно прислать один раз (для самого первого ДЗ). Для последующих ДЗ просто сообщайте, что оно готово и можно проверять
2. Учитесь грамотно формулировать свой вопрос: "у меня не получается" может иметь тысячи причин. Пишите больше подробностей о том, что вы сделали, что конкретно не получилось, какие появляются ошибки. Присылайте в чат скрины с этими ошибками
3. При выполнении ДЗ используйте только те темы, которые изучались в текущем уроке
4. Все задания выполняйте в разных классах
5. Код пишите только **ВНУТРИ** метода `main` (для каждого класса метод `main` будет своим)
6. Ввод с клавиатуры, методы класса `Math` или `Random` пока не используйте (но, если вы знаете про них и хотите использовать — дерзайте)
7. Так должна выглядеть структура ваших папок и файлов

![tree](https://user-images.githubusercontent.com/29703461/166162351-44d7f0fc-60ee-45b1-85f5-c1310216e783.png)

## Немного мотивации
- [Shia LaBeouf Motivation for Coding](https://youtu.be/J1usv2Hn-pU)
- [Мотивация для программистов](https://www.youtube.com/watch?v=NOVaNe3jx6c)
- [Речь Стива Джобса Перед выпускниками Стенфорда](https://www.youtube.com/watch?v=WVz9E7o1mmk)
- [Мотивационный совет от Стива Джобса](https://www.youtube.com/watch?v=Z2qSUZ1o47U)
- [12 минут сильнейшей мотивации. Перелом сознания](https://www.youtube.com/watch?v=69MkvKrraC0)
