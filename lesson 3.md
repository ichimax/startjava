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

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 1. <a name="1">[Механизм пакетов (package) в Java](https://drive.google.com/file/d/1dzZwKVirUys88V5_CVM0RfQ4iQcQ0cIq/view?usp=sharing)</a>
![package](https://user-images.githubusercontent.com/29703461/166163450-3366ac0b-274d-416e-b4af-e31f805e8cd9.png)

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
- [javac — документация по Java-компилятору](https://docs.oracle.com/en/java/javase/19/docs/specs/man/javac.html)
- [java — документация по java-лаунчеру](https://docs.oracle.com/en/java/javase/19/docs/specs/man/java.html)

## ![video](https://user-images.githubusercontent.com/29703461/81982928-d556fb00-9632-11ea-9794-ea198832d674.png) 3. <a name="3">[.gitignore](https://drive.google.com/file/d/1cJVmgrIfLo4iNDhfNkrdkkSZUKszzApN/view?usp=sharing)</a>
**Материалы:**
- [Игнорирование файлов в git](https://youtu.be/fzmCx6FLLu0)
- [Git — игнорирование файлов](https://www.youtube.com/watch?v=EjRQ8qccLCQ) (youtube)
- [Документация по gitignore](https://git-scm.com/docs/gitignore)
- [Как создать файл .gitignore в Windows](https://ru.stackoverflow.com/questions/438367/Как-создать-файл-gitignore-в-windows/438370)
- [Что должно и не должно быть в .gitignore](https://ru.stackoverflow.com/questions/474556/Что-должно-и-не-должно-быть-в-gitignore-для-любого-языка-и-ide)

## 4. <a name="4">Ответы на вопросы</a>

> Когда я компилирую, то почему-то в папке out не создается такая же структура папок, как и в папке src. При этом class-файлы появляются в корне папки out

Забыли добавить `package` в ваши классы

[Компилятор не создает папки для *.class](https://ru.stackoverflow.com/questions/451524/java-не-создает-папки-для-class)

> Я случайно занес в индекс Git папку out с class-файлами. И, если я не уберу ее, то при пуше она уйдет на GitHub. Как сделать так, чтобы Git ее не видел и не индексировал?

Написать в консоли `git rm -r --cached out`, а после занести папку `out` в файл `.gitignore`

[Удаление файлов из индекса git'а](https://git-scm.com/book/ru/v2/%D0%9E%D1%81%D0%BD%D0%BE%D0%B2%D1%8B-Git-%D0%97%D0%B0%D0%BF%D0%B8%D1%81%D1%8C-%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B9-%D0%B2-%D1%80%D0%B5%D0%BF%D0%BE%D0%B7%D0%B8%D1%82%D0%BE%D1%80%D0%B8%D0%B9#:~:text=%D0%BA%D0%BE%D0%BC%D0%BC%D0%B8%D1%82%20%D0%BD%D0%B5%D0%B6%D0%B5%D0%BB%D0%B0%D1%82%D0%B5%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5%20%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D1%8F.-,%D0%A3%D0%B4%D0%B0%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5%20%D1%84%D0%B0%D0%B9%D0%BB%D0%BE%D0%B2,-%D0%94%D0%BB%D1%8F%20%D1%82%D0%BE%D0%B3%D0%BE%20%D1%87%D1%82%D0%BE%D0%B1%D1%8B)

## 5. <a name="5">Домашнее задание</a>
- **[Домашнее задание](https://docs.google.com/document/d/1UGPow_Tqdq3GjOvBBkEsiWUu5R1NMcE83tW-Cnosu8E/edit?usp=sharing)**
- Так должна выглядеть структура ваших папок и файлов (на GitHub папку `out` не загружайте)
 
![tree2](https://user-images.githubusercontent.com/29703461/166163390-4cc031ba-f946-47a8-b83e-861d1409f812.png)

## 6. <a name="6">Опросники</a>
- [Итоговый тест](https://forms.gle/TqeeTy7QvUyCpsaj9) позволит вам проверить, насколько хорошо вы освоили пройденные темы
- В этом небольшом [опроснике](https://forms.gle/wrnyKTeMoDJggTNW7) вы сможете поделиться своими впечатлениями (анонимно) по поводу третьего урока: что (не)понравилось, как его можно улучшить и тд. Ваши ответы помогут нам доработать урок, сделав его еще лучше! 
