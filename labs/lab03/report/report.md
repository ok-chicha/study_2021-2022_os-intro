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

Научиться оформлять отчёты с помощью легковесного языка разметки Markdown.

# Задание

1. Сделайте отчёт по предыдущей лабораторной работе в формате Markdown.
2. В качестве отчёта просьба предоставить отчёты в 3 форматах: pdf, docx и md (в архиве,поскольку он должен содержать скриншоты, Makefile и т.д.)



# Выполнение лабораторной работы

1. Создаем титульный лист. (рис. [-@fig:001])

![титульный лист](image/1lab3.png){ #fig:001 width=70% }

2. Формулируем цель лабораторной работы №2. (рис. [-@fig:002])

![цель работы](image/2lab3.png){ #fig:002 width=70% }

3. Формулируем задания работы. (рис. [-@fig:003])

![задания работы](image/3lab3.png){ #fig:003 width=70% }

3. Описываем результаты выполнения заданий лабораторной работы № 2:
 - скриншоты фиксирубщие выполнение работы;
 - ответы на контрольные вопросы
.(рис. [-@fig:004])( рис. [-@fig:005])

![описание действий в лабораторной работе 2](image/4lab3.png){ #fig:004 width=70% }

![контрольные вопросы](image/6lab3.png){ #fig:005 width=70% }

4. написание выводы согласованного с задание работы. ( рис. [-@fig:006])

![вывод](image/5lab3.png){ #fig:006 width=70% }

5. преобразовываем файл в форматы pdf и docx. ( рис. [-@fig:007])

![преобразование файла](image/7lab3.png){ #fig:007 width=70% }

# Вывод

Приобрела практические навыки оформления отчетов с помощью легковесного языка разметки Markdown. 




