---
## Front matter
title: "Отчёта по лабораторной работе No11"
author: "Cиссе Мохамед Ламин"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---
# Цель работы
Приобрестни навыки работы с файлами в языке NASM и научиться управлять правами доступа к файлам.

# Выполнение лабораторной работы
Создайте каталог для программам лабораторной работы No 11, перейдите
в него и создайте файл lab11-1.asm и readme.txt. (рис. [-@fig:001])

![Текст программы](image/01.png){ #fig:001 width=70% }

Введите в файл lab11-1.asm текст программы из листинга 11.1 (Программа
записи в файл сообщения). Создайте исполняемый файл и проверьте его
работу.рис. ([-@fig:002])

![работа программы](image/02.png){ #fig:002 width=70% }

 Проассемблируем программу и проверим ее работу(рис. [-@fig:003])

![работа программы](image/03.png){ #fig:003 width=70% }

Запретим исполнение для файла lab11-1.(рис. [-@fig:004])

![как и ожидалось, мы не смогли исполнить этот файл](image/04.png){ #fig:004 width=70% }

если запретить исполнение файла, то исполнить его станет невозможно.

Когда мы разрешим исполнение файла с расширением .asm и собственно исполним его, то мы увидем множество ошибок, ведь этот файл не предназначен для такого использования.(рис. [-@fig:005])

![Ошибки исполнения файла lab11-1.asm](image/05.png){ #fig:005 width=70% }

Зададим файлу readme.txt права использования как во варианте 17 и проверим как получилось.(рис. [-@fig:006])

![Права доступа к файлу readme.txt r-x -wx rw-](image/06.png){ #fig:006 width=70% }

# Задания для самостоятельной работы
![часть текста программы](image/07.png){ #fig:007 width=70% }

![работа полученной програмы](image/08.png){ #fig:008 width=70% }

# Выводы
были преобретены навыки по работе с файлами в NASM и правами доступа к файлам.
