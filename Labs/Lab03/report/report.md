---
# Front matter
lang: ru-RU
title: "Отчет по Лабораторной Работе №3"
subtitle: "Моделирование стохастических процессов"
author: "Озьяс Стев Икнэль Дани"

## Pdf output format
toc: true # Table of contents
toc-depth: 2
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
lofTitle: "Цель Работы"
lotTitle: "Ход Работы"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Моделирование стохастических процессов

# Выполнение лабораторной работы


## Задача 1

На базе файла shablon.tcl, создал файл lab3.tcl и отредактировал его.

![Редактирование файла lab3.tcl](image/image1.png){ #fig:001 width=70% }

Запустил его командой $ns$.

![Запуск симулятора lab3.tcl](image/image2.png){ #fig:002 width=70% }


## Задача 2


В каталоге с проектом создал отдельный файл $graph_plot$. Открыл его на редактирование и добавил следующий код, обращая внимание:

![Редактирование файла graph_plot](image/image3.png){ #fig:003 width=70% }


## Задача 3


Сделал файл исполняемым. После компиляции файла с проектом, запустил скрипт в созданном файле graph_plot, который создаст файл qm.pdf с результатами моделирования:

![ График поведения длины очереди](image/image4.png){ #fig:004 width=70% }


# Выводы

В результате проделанной лабораторной работы выпольнили моделирование стохастических процессов с помощью средства имитационного моделирования NS-2 и GNUplot.