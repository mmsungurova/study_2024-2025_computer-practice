---
## Front matter
title: "Компьютерный практикум по статистическому анализу данных"
subtitle: "Лабораторная работа № 7. Введение в работу с данными"
author: "Сунгурова Мариян Мухсиновна"

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
lot: false # List of tables
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

# Введение

**Цель работы**

Основной целью работы является освоение специализированных пакетов Julia для обработки данных.

**Задачи**

1. Используя Jupyter Lab, повторите примеры.
2. Выполните задания для самостоятельной работы.

# Теоретическое введение

Julia — высокоуровневый свободный язык программирования с динамической типизацией, созданный для математических вычислений[@julialang]. Эффективен также и для написания программ общего назначения. Синтаксис языка схож с синтаксисом других математических языков, однако имеет некоторые существенные отличия.

Для выполнения заданий была использована официальная документация Julia[@juliadoc].

# Выполнение лабораторной работы

Выполним примеры из лабораторной работы для изучения циклов и функций(рис. @fig:001 -  @fig:015)


![Примеры Считывание данных](image/1.JPG){#fig:001 width=70%}


![Примеры Считывание данных ](image/2.JPG){#fig:002 width=70%}


![Примеры Запись данных в файл](image/3.JPG){#fig:003 width=70%}


![Примеры Словари](image/4.JPG){#fig:004 width=70%}


![Примеры DataFrames](image/5.JPG){#fig:005 width=70%}


![Примеры RDatasets](image/6.JPG){#fig:006 width=70%}


![Примеры Missing type](image/7.JPG){#fig:007 width=70%}


![Примеры Fileio](image/8.JPG){#fig:008 width=70%}

![Примеры Кластеризация](image/9.JPG){#fig:009 width=70%}

![Примеры Кластеризация](image/10.JPG){#fig:010 width=70%}

![Примеры Кластеризация](image/11.JPG){#fig:011 width=70%}

![Примеры Кластеризация](image/12.JPG){#fig:012 width=70%}

![Примеры Метод главных компанент](image/13.JPG){#fig:013 width=70%}

![Примеры Линейная регрессия](image/14.JPG){#fig:014 width=70%}

![Примеры Линейная регрессия](image/15.JPG){#fig:015 width=70%}


Затем выполним задания(рис. @fig:016 - @fig:015)

![Задания 1 ](image/16.JPG){#fig:016 width=70%}

![Задания 1](image/17.JPG){#fig:017 width=70%}

![Задания 2](image/18.JPG){#fig:018 width=70%}









# Выводы

В результате выполнения данной лабораторной работы было освоено использование специализированных пакетов Julia для обработки данных.

# Список литературы{.unnumbered}

::: {#refs}
:::

