---
## Front matter
title: "Лабораторная работа 3"
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

Цель работы научится оформлять отчеты с помощью легковесного языка разметки Markdown.

# Задание

1. сделайте отчет по предыдущей лабораторной работе в формате Markdown.
2. В качестве отчета предоставить отчеты в 3 форматах: pdf, docx и md.

# Выполнение лабораторной работы

Создаем учетную запись на https://github.com и заполняем основные данные . Устанавливаем программное обеспечение git-flow , используя команды «wget», «chmod», и «sudo». (рис. [-@fig:001])

![установка програмного обеспечения git-flow](image/1.png){ #fig:001 width=70% }

Установка gh. Переходим к базовой настройке git , для этого задаем имя и email владельца репозитория, настраиваем utf-8 в выводе сообщений git,а также верификацию и подписание коммитов git, задаем имя начальной ветки (master), устанавливаем параметры autocrlf и safecrlf. (рис. [-@fig:002])

![базовая настройка git](image/2.png){ #fig:002 width=70% }

Создаем ключи ssh по алгоритму rsa с клечём размером 4096 бит .(рис. [-@fig:003])

![создание ключей ssh](image/3.png){ #fig:003 width=70% }

Генерируем ключи pgp командой «gpg --full-generate-key» и из предложенных опций выбираем:
- тип RSA and RSA;
- размер 4096;
- выберите срок действия - 0 (срок действия не истекает никогда).
- Имя (okchichkina).
- Адрес электронной почты(olka.chichkina@gmail.com) (рис. [-@fig:004])

![Генерация ключей pgp](image/4.png){ #fig:004 width=70% }

Для добавления ключа pgp в github нужно вывести список ключей и скопировать отпечаток приватного ключа  (86E5C166DD4341D1). Далее мы вставляем полученный отпечаток в команду для копирования ключа pgp, и получаем команду вида «gpg –armor –export 86E5C166DD4341D1 ». после этого мы подключаем полученный ключ на github. (рис. [-@fig:005])

![добавление ключа pgp к github](image/5.png){ #fig:005 width=70% }

Используя email, указываем git применять его при подписи коммитов (рис. [-@fig:006])

![подписи коммитов](image/6.png){ #fig:006 width=70% }

Начинаем выполнять настройку gh, для этого авторизовываемся и отвечаем на вопросы утилиты .(рис. [-@fig:007])

![настройку gh](image/7.png){ #fig:007 width=70% }

Переходим к созданию шаблона рабочего пространства и настройке каталога курса. (рис. [-@fig:008])

![создание шаблона рабочего пространства](image/8.png){ #fig:008 width=70% }
 
# Выводы

научились выполнять отчеты с помощью легковесного языка Markdown.


