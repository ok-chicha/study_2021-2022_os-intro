---
## Front matter
title: "лабораторная работа №4"
subtitle: "Дисциплина операционные системы"
author: "Чичкина Ольга Константиновна"

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

Приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.

# Выполнение лабораторной работы

Определим полное имя своего домашнего каталога и далее в этом каталоге :
 1. переходим в каталог /tmp (рис. [-@fig:001])

![домашний каталог и каталог tmp](image/1lab4.png){ #fig:001 width=70% }

 2. выводим на экран содержимое каталога /tmp с помощью команды ls с различными опциям
  - ls -a ( отображает имена скрытых файлов)
  - ls -F ( отображает типы файлов)
  - ls -l ( ОТОБРАЖАЕТ ПОДРОБНУЮ ИНФОРМАЦИЮ О ФАЙЛАХ И КАТАЛОГАХ) (рис. [-@fig:002] [-@fig:003] [-@fig:004])
 
![ls1](image/2lab4.png){ #fig:002 width=70% }

![ls2](image/3lab4.png){ #fig:003 width=70% }
 
![ls3](image/4lab4.png){ #fig:004 width=70% }

 3. определяем есть ли в каталоге /var/spool подкаталог с именем cron, такого подкаталога не сущетсвует.(рис. [-@fig:005])

![каталог spool](image/5lab4.png){ #fig:005 width=70% }

 4. переходим в домашний каталог и определяем владельца файлов и каталогов, владельцем является okchichkina. (рис. [-@fig:006])

![домашний каталог](image/6lab4.png){ #fig:007 width=70% }

сооздаем в домашнем каталоге новый каталог newdir и в нем каталог morefun(рис. [-@fig:007])

![newdir](image/7lab4.png){ #fig:007 width=70% }

В домашнем каталоге создаем одной командой три новых каталога с именами
letters, memos, misk. Затем удаляем эти каталоги одной командой.(рис. [-@fig:008])

![три каталога](image/8lab4.png){ #fig:008 width=70% }

Удаляем ранее созданный каталог ~/newdir командой rm. Проверяем
был ли каталог удалён. (рис. [-@fig:009])

![удаление newdir](image/9lab4.png){ #fig:009 width=70% }

С помощью команды man узнаем основные опции команд ls, cd, pwd, mkdir, rmdir, rm. (рис. [-@fig:010])

![команда man](image/10lab4.png){ #fig:010 width=70% }

Используя информацию, полученную при помощи команды history, выполниv модификацию и исполнение нескольких команд из буфера команд(рис. [-@fig:011])

![history](image/12lab4.png){ #fig:011 width=70% }

# контрольные вопросы

1. Командная строка представляет собой программное средство ввода команд пользователем и получения результатов их выполнения на экране.
2. Для определения абсолютного пути к текущему каталогу используется
команда pwd (print working directory).
 Пример (абсолютное имя текущего каталога пользователя dharma):
  pwd
 результат:
  /afs/dk.sci.pfu.edu.ru/home/d/h/dharma
3. Команда ls используется для просмотра содержимого каталога.
 Можно также получить информацию о типах файлов (каталог, исполняемый файл,ссылка), для чего используется опция F. При использовании этой опции в поле имени выводится символ, который определяет тип файла . символ `/' после имен подкаталогов и символ `*' после имен исполняемых файлов.
 пример :
  ls -F
 результат выполнения:
  repeat* test1   test2   words/
4. -a или -all
Выводить все файлы, включая скрытые файлы.


# Выводы

Приобрела практические навыки взаимодействия пользователя с системой посредством командной строки.


