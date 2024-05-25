> ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) — эта иконка означает, что рядом с ней находится ссылка, содержащая видеоурок: кликайте на нее для его просмотра

## [Отзывы выпускников о курсе](https://vk.com/topic-18505771_38447031?offset=100)
## [Демонстрация проверки ДЗ наставником](https://youtu.be/H_PYOW9Qq80?si=isPC3-aYYPhDWL5B)

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
1. [Итоговые домашние задания](#10)
1. [Опросники](#11)
1. [Общие рекомендации по выполнению ДЗ](#12)

# [Видеообзор курса StartJava](https://youtu.be/vM1ygW7pKTE)
- На данный момент обучение проводится в Slack в индивидуальном режиме
- Обязательно читайте книги из [списка](https://topjava.ru/blog/spisok-knig-dlya-nachinayushchego-java-programmista) параллельно изучаемым темам

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 1. <a name="1">[Подготовка рабочего окружения](https://drive.google.com/file/d/1gWrBFrly3BdXKq868Xr0QkGtpM9FCmI4/view?usp=sharing)</a>

- [Установите и настройте Java](https://topjava.ru/blog/ustanovka-i-nastroyka-java)
- Скачайте и установите [Sublime Text 4](https://www.sublimetext.com/download). Именно в нем мы будем писать наши программы (с четвертого урока перейдем на IntelliJ IDEA)

**[Отключите](https://chromefaq.ru/nastrojki/kak-perevodit-stranitsy-v-google-chrome-s-anglijskogo-na-russkij#i-6) в браузере автоперевод страниц. Из-за него уроки могут отображаться некорректно**

**Материалы:**
- [Знакомство с языком Java](https://www.youtube.com/live/QGHGR0xEcFA?si=xW98gPEVGZX_UrG5)
- [Что такое JDK? Введение в средства разработки Java](https://topjava.ru/blog/what-is-the-jdk)
- [Что такое JRE? Введение в среду выполнения Java](https://topjava.ru/blog/what-is-the-jre)
- [Что такое JVM? Знакомство с виртуальной машиной Java](https://topjava.ru/blog/what-is-the-jvm)
- Отчет о популярности Java-технологий в [2019](https://topjava.ru/blog/sostoyanie-java-v-2019-godu), в 2023 ([1](https://drive.google.com/file/d/1KAqubG1ETRfRioEcM46M-OKOh2ZNpzJQ/view?usp=sharing), [2](https://drive.google.com/file/d/14V5UBnbGI7pSa2_kIir36eilF36LiZOD/view?usp=sharing), [3](https://www.jetbrains.com/ru-ru/lp/devecosystem-2022/java/))

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
- [Настройте](https://topjava.ru/blog/nastroyka-sublime-text-dlya-java#7) проверку правописания для Sublime Text

**Материалы:**
- [Обзор и настройка Sublime Text](https://youtu.be/xWhTf_o86Lg) — видео дано для ознакомления с возможностями редактора. Это не значит, что вам нужно делать все то, что делает его автор (youtube)
- [Установка плагина Terminal для SublimeText](https://youtu.be/9cFW481D2lU) (youtube) — можно использовать либо этот плагин, либо `Terminus`

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 3. <a name="3">[Ручная компиляция и запуск программы](https://drive.google.com/file/d/1u0jyGJkFFLUwfj0c21uY2i2louNtIm_3/view?usp=sharing)</a>
Для компиляции и запуска программы необходимо в консоли перейти в папку, в которой находится файл `MyFirstApp.java`, и ввести последовательно следующие команды:
- `javac MyFirstApp.java` — компиляция java-файла
- `java MyFirstApp` — запуск программы

Для однофайловых программ, начиная с Java 11, процесс компиляции и запуска можно совместить в одной команде:
- `java MyFirstApp.java`

Для того, чтобы русский текст корректно отображался в консоли, компилируйте свои программы с помощью специального параметра `javac -encoding utf8 имя_класса.java`

Более подробно об этом рассказывается в статье [Компиляция и запуск Java-программ](https://topjava.ru/blog/kompilyatsiya-i-zapusk-programm-na-java)

А из статьи ["Основы командной строки для Java-программиста"](https://topjava.ru/blog/osnovy-komandnoy-stroki-dlya-java-programmista) вы узнаете о самых нужных и часто используемых командах консоли для работы с файловой системой 

**Материалы:**
- [Getting Started with Java](https://dev.java/learn/getting-started/)
- [Введение в командную строку Windows](https://www.youtube.com/user/Iidsp/videos) (youtube)

## 4. <a name="4">Этапы компиляции и запуска</a>
![Frame 303](https://github.com/ichimax/startjava/assets/29703461/613d6100-8fc1-4054-9811-cf143b61d32c)

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
- [Про размеры типов данных](https://youtu.be/3BmznLJAgaA?t=782)

![var](https://user-images.githubusercontent.com/29703461/155842985-5fae137b-3967-4fe6-893c-0d2a018815a5.png)

- **Домашнее задание:**
  - Разберитесь с [Git/GitHub](https://github.com/ichimax/startjava/blob/master/lesson%201.md#9)
  - Пришлите наставнику ссылку на удаленный репозиторий с решенными ДЗ
  - ["Именование переменных"](https://docs.google.com/document/d/1Dv-eo8acvOVFJtUVbaWd1Mfb77Q1IiTlhepgy56qMbc/edit?usp=sharing)
  - ["Примитивные типы данных"](https://docs.google.com/document/d/1kJqeCC-fKWUjBjrmHJ1mjDu45SGRL39Q5vW4DmLJflA/edit?usp=sharing)

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
- Циклы в Java [1](https://timeweb.cloud/tutorials/java/cikly-v-java-osnovy-raboty), [2](https://vertex-academy.com/tutorials/ru/cikly-v-java/)
- [Оператор while](https://youtu.be/15PjODTSTaw) (youtube)
- [Оператор for](https://youtu.be/UYbdAmgcNVc) (youtube)

**Домашнее задание:**
- **[Домашние задания по теме "Циклы: for, while, do while"](https://docs.google.com/document/d/1lHSSOzARTx6tfD-4MV-t41S5bnvdNw5hczkQPT05png/edit?usp=sharing)**
- **Покажите ДЗ наставнику**

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 9. <a name="9">[Система управления версиями Git](https://drive.google.com/file/d/1IMw7DA_lodW2GueWpU1nMUmYx0pnlPGA/view?usp=sharing)</a>
![image](https://user-images.githubusercontent.com/29703461/154850409-7a618576-1105-48a1-9e32-88a34e87693b.png)

- [Установите и настройте Git/GitHub](https://topjava.ru/blog/vvedeniye-v-git-github-ustanovka-i-nastroyka)

**Материалы:**
  - [Базовый курс по обучению Git](https://www.youtube.com/playlist?list=PLIU76b8Cjem5B3sufBJ_KFTpKkMEvaTQR) (youtube)
  - [Git. Быстрый старт](https://www.youtube.com/watch?v=4-NX17Ip-xQ&list=PLmRNNqEA7JoM77hOJkPrLOfJQGizCLR3P) (youtube)
  - Интерактивные Git-обучалки: [1](https://githowto.com/ru), [2](http://learngitbranching.js.org)
  - [Официальная книга про Git](https://git-scm.com/book/ru/v2)
  
### Настройка локального репозитория
Более подробно об этом рассказывается в статье [Введение в Git/GitHub: базовые команды](https://topjava.ru/blog/vvedeniye-v-git-github-bazovyye-komandy).

- Создайте в удобном для вас месте папку под названием `StartJava`. В ней будет храниться ваш код
- Создайте на GitHub репозиторий с названием `startjava`
- Напишите в консоли (при этом консоль должна быть открыта в папке `startjava`): 
  - `git init` — создание локального репозитория
  - `git status` — вывод состояния файлов
  - добавьте адрес созданного на GitHub репозитория в git — `git remote add origin url_на_ваш_startjava-репозиторий.git`
  - проверьте, добавился он или нет — `git remote -v`

### Рекомендации по Git
1. Последовательность стандартных шагов при работе с Git:
   - `git add файл_с_кодом.java` — добавляем файлы/изменения в git (файлы с расширением `class` не добавляйте)
   - `git commit -m "краткое описание изменений, которые вы внесли в программу"` — фиксируем (коммитим) изменения
   - `git push -u origin master` — [устанавливаем связь](https://qna.habr.com/q/118865) между локальной и удаленной веткой master
1. На GitHub можно отправлять не только файлы с расширением `java`, но и папки, например, `Lesson 1` (при этом они не должны быть пустыми)
1. Если вы столкнулись с проблемами при использовании Git, то статья ["Ошибки использования Git"](https://topjava.ru/blog/vvedeniye-v-git-oshibki-ispolzovaniya-ch-9) поможет их решить

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 10. <a name="10">[Итоговые домашние задания](https://drive.google.com/file/d/1Svgm_03td3Aj_MeVt-MBqSCv-PEhXD0A/view?usp=sharing)</a>

- **[Итоговые домашние задания](https://docs.google.com/document/d/1m6y5qBMfwKjm0DIo3JYqQ9_QNyhroDvsRAirEyDEP7s/edit?usp=sharing)**

<details>
<summary>Так должна выглядеть структура ваших папок и файлов</summary>
    
![tree](https://github.com/ichimax/startjava/assets/29703461/47ca8fc6-3f00-4c24-a07d-0e2416f12eb6)
</details>

## 11. <a name="11">Опросники</a>
- [Итоговый тест](https://forms.gle/YFc2pf6qZw6jdfXM7) позволит вам проверить, насколько хорошо вы освоили пройденные в уроке темы
- В этом небольшом [опроснике](https://forms.gle/dsthsvh1tRhdJyhu9) вы сможете поделиться своими впечатлениями (анонимно) по поводу первого урока: что (не)понравилось, как его можно улучшить и тд. Ваши ответы помогут нам доработать урок, сделав его еще лучше!

## 12. <a name="12">Общие рекомендации по выполнению ДЗ</a>

1. [Правила](https://github.com/ichimax/startjava/blob/master/rules.md) проверки ДЗ наставником
1. Ментору ссылку на репозиторий достаточно прислать один раз (для самого первого ДЗ). Для последующих ДЗ просто сообщайте, что оно готово и можно проверять
1. При выполнении ДЗ используйте только те темы, которые изучались в текущем уроке
1. Ввод с клавиатуры, методы класса `Math` или `Random` пока не используйте (но, если вы знаете про них и хотите использовать — дерзайте)

## Немного мотивации
- [Как приучить себя к дисциплине и осуществлять свои планы](https://youtu.be/wbItXmjm7tY?si=RceAgonMsijaz3KD)
- [Shia LaBeouf Motivation for Coding](https://youtu.be/J1usv2Hn-pU)
- [Мотивация для программистов](https://www.youtube.com/watch?v=NOVaNe3jx6c)
- [Речь Стива Джобса Перед выпускниками Стенфорда](https://www.youtube.com/watch?v=WVz9E7o1mmk)
- [Мотивационный совет от Стива Джобса](https://www.youtube.com/watch?v=Z2qSUZ1o47U)
- [12 минут сильнейшей мотивации. Перелом сознания](https://www.youtube.com/watch?v=69MkvKrraC0)
- [Почему мне так сложно учиться программировать?](https://youtu.be/TtT8UNK0sGg)
- [Простой прием стать программистом быстрее](https://youtu.be/iw3E-Gdncwc)
