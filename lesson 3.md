# Занятие третье

## Разбор домашнего задания
- ![video](https://user-images.githubusercontent.com/29703461/81983788-359a6c80-9634-11ea-9b47-09a56fd3d999.png) [Jaeger (setters)](https://drive.google.com/file/d/1_ljcNYoajX_N48bYCRBAQOCR18telTUp/view?usp=sharing)
- ![video](https://user-images.githubusercontent.com/29703461/81983788-359a6c80-9634-11ea-9b47-09a56fd3d999.png) [Jaeger (constructors)](https://drive.google.com/file/d/1j-7-cA_WmlCQC_-2MgAMuQTUpKKE4ylt/view?usp=sharing)
- ![video](https://user-images.githubusercontent.com/29703461/81983788-359a6c80-9634-11ea-9b47-09a56fd3d999.png) [Калькулятор](https://drive.google.com/file/d/1v1MaEFTnHSpYsy4pF0a1D6kiJqQaf2he/view?usp=sharing)
- ![video](https://user-images.githubusercontent.com/29703461/81983788-359a6c80-9634-11ea-9b47-09a56fd3d999.png) [Угадай число](https://drive.google.com/file/d/1AFfvUiPiR87noEFrX8n7y9Tet57oHvEq/view?usp=sharing)

## Темы третьего занятия
1. [Механизм пакетов (package) в Java](#1)
1. [Компиляция Java-программ. Часть II](#2)
1. [.gitignore](#3)
1. [Ответы на вопросы](#4)
1. [Домашнее задание](#5)
1. [Опросники](#6)
1. [Советы по выполнению домашнего задания](#7)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 1. <a name="1">[Механизм пакетов (package) в Java](https://drive.google.com/file/d/1dzZwKVirUys88V5_CVM0RfQ4iQcQ0cIq/view?usp=sharing)</a>
![package](https://user-images.githubusercontent.com/29703461/112764220-364fad80-9010-11eb-8ef1-44b5f4054b4d.png)

**Материалы:**
- [Пакеты в Java](https://ru.wikipedia.org/wiki/Package_(Java)) (wiki)
-	[Зачем нужны пакеты в Java и что это такое](http://pr0java.blogspot.ru/2015/06/java.html)
-	[Пакеты](https://www.youtube.com/watch?v=a6KGNASOtK8) (youtube)
- [Правила именования пакетов](https://ru.stackoverflow.com/questions/728735/Почему-пакеты-в-java-принято-называть-в-обратную-сторону-доменного-имени)
- [Reverse domain name notation](https://en.wikipedia.org/wiki/Reverse_domain_name_notation)
- [Packages](https://docs.oracle.com/javase/tutorial/java/package/index.html)
- [Стандартные пакеты и классы Java: официальная документация](https://docs.oracle.com/javase/8/docs/api/) (eng)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 2. <a name="2">[Компиляция Java-программ. Часть II](https://drive.google.com/file/d/13re6jwLbagQaIkmBPr3LNUc3hIEGUbiZ/view?usp=sharing)</a>
**Материалы:**
- [Работа с Java в командной строке](https://habr.com/post/125210/)
- [javac — Java programming language compiler](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/javac.html)
- [java — Launches a Java application](https://docs.oracle.com/javase/8/docs/technotes/tools/windows/java.html)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 3. <a name="3">[.gitignore](https://drive.google.com/file/d/1cJVmgrIfLo4iNDhfNkrdkkSZUKszzApN/view?usp=sharing)</a>
**Материалы:**
- [Игнорирование файлов в git](https://youtu.be/fzmCx6FLLu0)
- [Git — игнорирование файлов](https://www.youtube.com/watch?v=EjRQ8qccLCQ) (youtube)
- [Официальная документация — gitignore](https://git-scm.com/docs/gitignore)
- [Как создать файл .gitignore в Windows](https://ru.stackoverflow.com/questions/438367/Как-создать-файл-gitignore-в-windows/438370)
- [Что должно и не должно быть в .gitignore](https://ru.stackoverflow.com/questions/474556/Что-должно-и-не-должно-быть-в-gitignore-для-любого-языка-и-ide)

## 4. <a name="4">Ответы на вопросы</a>

> Когда я компилирую, то почему-то в папке out не создается такая же структура папок, как и в папке src. При этом class-файлы появляются в корне папки out

Забыли добавить `package` в ваши классы

[Компилятор не создает папки для *.class](https://ru.stackoverflow.com/questions/451524/java-не-создает-папки-для-class)

> Я случайно занес в индекс git папку out с class-файлами. И, если я не уберу ее, то при пуше она уйдет на github. Как сделать так чтобы git ее не видел и не индексировал?

Написать в консоли `git rm -r --cached out`, а после занести папку `out` в файл `.gitignore`

[Удаление файлов из индекса git'а](https://git-scm.com/book/ru/v1/Основы-Git-Запись-изменений-в-репозиторий#Удаление-файлов)

## 5. <a name="5">Домашнее задание</a>

> Перед отправкой домашнего задания на проверку обращайте внимание на [`Советы по выполнению домашнего задания`](#6), которые содержат ряд полезных подсказок и разъяснений
- Наведите порядок в папках и файлах в соответствии со структурой, представленной на картинке ниже
- Создайте в корне проекта (на одном уровне с папкой `src` и `out`) файл с именем `.gitignore`
- Добавьте в `.gitignore` папку с class-файлами
- Во всех классах пропишите названия пакетов
- После всех изменений вам необходимо:
  - добавить папку `src` в индекс git'а с помощью `add`
  - удалить из индекса git'а папки, которые там были ранее — `git rm -r --cached "Lesson 1" "Lesson 2"`, т.к. структура файлов изменилась, и ее нужно перезаписать
  - выполнить коммит
  - сделать принудительный (force) пуш `git push -f`, который заменит текущую структуру файлов и папок на GitHub на новую
- Скомпилируйте и запустите все свои программы
- Покажите наставнику:
    - скрин консоли с компиляцией и запуском `Игры`
    - скрин с выводом дерева каталогов и файлов, начиная от папки `startjava` (для этого используйте в консоли команду `tree /F`)

## 6. <a name="6">Опросники</a>
- [Итоговый тест](https://forms.gle/TqeeTy7QvUyCpsaj9) позволит вам проверить, насколько хорошо вы осовили пройденные темы
- В этом небольшом [опроснике](https://forms.gle/wrnyKTeMoDJggTNW7) вы сможете поделиться своими впечатлениями (анонимно) по поводу третьего урока: что (не)понравилось, как его можно улучшить и тд. Ваши ответы помогут нам доработать урок, сделав его еще лучше!

## 7. <a name="7">Советы по выполнению домашнего задания
    
- Не забудьте добавить в git (с помощью `add`) файл `.gitignore`
- `-sourcepath имя_директории` — данный ключ позволяет упростить компиляцию программы, состоящей из нескольких файлов
- Так должна выглядеть структура ваших папок и файлов (на GitHub папку `out` не загружайте)

  ![tree2](https://user-images.githubusercontent.com/29703461/112763927-21264f00-900f-11eb-91b0-63e6bc0c558e.png)
