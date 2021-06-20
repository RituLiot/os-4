---
# Front matter
lang: ru-RU
title: Знакомство с операционной системой Linux
subtitle: ЛР по ОС №4
author: Аникин Константин Сергеевич
group: НПИбд-01-20

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цели работы

Познакомиться с операционной системой Linux, 
получить практические навыки работы с консолью и 
некоторыми графическими менеджерами 
рабочих столов операционной системы.

# Задание

- Ознакомиться с теоретическим материалом.

- Выполнить задание 

# Теоретическое введение 

[[1]](https://interface31.ru/tech_it/2014/09/linux-nachinayuschim-chast-1-pervoe-znakomstvo.html):

Для привыкшего к графическим инструментам Windows-администратора это может показаться сложным. 
Но следует твердо усвоить одну истину - консоль является единственным полноценным 
инструментом администрирования Linux и совсем не означает ограниченность в 
возможностях или неполноценность системы. Даже наоборот, командная строка 
позволяет выполнить многие задачи намного быстрее и проще, 
чем графические инструменты администрирования.

Linux, создававшийся по образу и подобию UNIX-систем, 
является полноценной системой и без графической оболочки, 
более того мы можем запустить, закрыть или вообще сменить 
графическую оболочку без какого-либо влияния на работоспособность 
системы и даже без ее перезагрузки. Завершили сеанс Gnome, 
запустили KDE, а потом и вовсе вышли в консоль. Поэтому все 
инструменты управления системой разработаны для использования 
в режиме командной строки. А все панели и графические инструменты 
являются всего лишь надстройкой над ними.

Краткий справочник команд Linux [[2]](https://hpc.icc.ru/documentation/cmnds.pdf)

# Выполнение лабораторной работы

Важное замечание: работу я делал на своей виртуальной машине 

3. Из моих изысканий о лучшей в мире CentOS я не понял, 

как переключиться на консоль при запуске, поэтому воспользовался

командой "sudo init 3" (рис. 1)

Если я правильно понял вопрос, доступна одна текстовая консоль,

но которую можно запустить шестью разными сеансами.

![](https://raw.githubusercontent.com/RituLiot/os-4/main/images/1.png)

*Рис. 1: Запуск в режиме текстовой консоли*

5. Заход в систему. Логин - соглашение по наименованию.

Пароль не отображается никакими символами. (рис. 2)

![](https://raw.githubusercontent.com/RituLiot/os-4/main/images/2.png)

*Рис. 2: Залогинился в систему*

4. Перешёл в другую консоль. Клавиши Alt+Fn, 

где n - номер консоли. (рис. 3)

![](https://raw.githubusercontent.com/RituLiot/os-4/main/images/3.png)

*Рис. 3: Перешёл в другую консоль*

6. Выход из консоли комбинацией Ctrl+D. Консоль перезапускается (рис. 4)

![](https://raw.githubusercontent.com/RituLiot/os-4/main/images/3.png)

*Рис. 4: Перезапуск консоли*

7. Переход в графический режим командой "sudo init 5"

Из-за моего метода перехода в графический режим комбинация

Ctral+Alt+F7 не работает. (рис. 5)

![](https://raw.githubusercontent.com/RituLiot/os-4/main/images/4.png)

*Рис. 5: Переход в графический режим*

10. Открытый текстовый редактор "Text Editor" (рис. 6)

![](https://raw.githubusercontent.com/RituLiot/os-4/main/images/6.png)

*Рис. 6: Text Editor*

10. Открытый браузер "Mozila Firefox" (рис. 7)

![](https://raw.githubusercontent.com/RituLiot/os-4/main/images/7.png)

*Рис. 7: Mozila Firefox*

10. Текстовый процессор у меня не установлен, устанавливать его не было

никакого желания. Аналогично с эмулятором консоли.

8. По умолчанию в CentOS установлен GNOME. Об этом я узнал уже

на момент написания отчёта, что могло бы помочь мне во время работы.

9. На моей машине не были установлены KDE, XCFE и Openbox 

(хотя в последнем я не уверен), и я обратился к интернету, как их установить.

Начать решил с GNOME, который предустановлен на CentOS, но об этом я узнал

лишь на момент написания отчёта. Для этого с помощью этой команды (рис. 8)

![](https://raw.githubusercontent.com/RituLiot/os-4/main/images/8.png)

*Рис. 8: Та команда*

установил кучу всего (рис. 9)

![](https://raw.githubusercontent.com/RituLiot/os-4/main/images/9.png)

*Рис. 9: Установка GNOME*

После чего ребутнул устройство. А оно не ребутнулось и выдало ошибку!(рис. 10)

![](https://raw.githubusercontent.com/RituLiot/os-4/main/images/10.png)

*Рис. 10: Ошибка при запуске*

Которую я не смог устранить. Пункт 9 не выполнен.

# Выводы

Работа выполнена на половину из-за отсутствия установленных 
графических сред и моей слабой психики

## Библиографический список

[1]: [Linux - начинающим. Часть 1. Первое знакомство](https://interface31.ru/tech_it/2014/09/linux-nachinayuschim-chast-1-pervoe-znakomstvo.html)

[2]: [Краткий справочник команд Linux](https://hpc.icc.ru/documentation/cmnds.pdf)
