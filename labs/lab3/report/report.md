---
## Front matter
title: "Компьютерный практикум по статистическому анализу данных"
subtitle: "Лабораторная работа № 3. Управляющие структуры"
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

Основная цель работы -- освоить применение циклов функций и сторонних для Julia пакетов для решения задач линейной алгебры и работы с матрицами.

**Задачи**

1. Используя Jupyter Lab, повторите примеры из раздела 3.2.
2. Выполните задания для самостоятельной работы (раздел 3.4).

# Теоретическое введение

Julia — высокоуровневый свободный язык программирования с динамической типизацией, созданный для математических вычислений.[@julialang]. Эффективен также и для написания программ общего назначения. Синтаксис языка схож с синтаксисом других математических языков, однако имеет некоторые существенные отличия.

Для выполнения заданий была использована официальная документация Julia[@juliadoc].

# Выполнение лабораторной работы

Выполним примеры из лабораторной работы для изучения циклов и функций(рис. @fig:001 -  @fig:005)

![Примеры. Циклы](image/1.JPG){#fig:001 width=70%}

![Примеры. Циклы](image/2.JPG){#fig:002 width=70%}

![Примеры. Циклы](image/3.JPG){#fig:003 width=70%}

![Примеры. Условия](image/4.JPG){#fig:004 width=70%}

![Примеры. Функции](image/5.JPG){#fig:005 width=70%}

![Примеры. Функции](image/6.JPG){#fig:006 width=70%}

![Примеры. Функции](image/7.JPG){#fig:007 width=70%}

![Примеры. Функции](image/8.JPG){#fig:008 width=70%}

В первом задании рассмотрим цикл for и создадим словарь, который будет содержать целые числа в качестве ключей и квадраты в качестве их пар-значений(рис. @fig:009)

![Задание 1](image/9.JPG){#fig:009 width=70%}

Создадим список с квадратами чисел от 1 до 100:

![Задание 1](image/10.JPG){#fig:010 width=70%}

Во втором задании напишем цикл на определение четности числа при помощи условных операторов

![Задание 2](image/11.JPG){#fig:011 width=70%}

В третьем напишем простую функцию прибавления единицы, 

![Задание 3](image/12.JPG){#fig:012 width=70%}

А в четвертом зададим матрицу A, каждый элемент которой увеличивается на единицу по сравнению с предыдущим(рис. @fig:013)

![Задание 4](image/13.JPG){#fig:013 width=70%}

Зададим матрицу A, найдем ее куб и изменим столбец(рис. @fig:0014)

![Задание 5](image/14.JPG){#fig:014 width=70%}

![Задание 5](image/15.JPG){#fig:015 width=70%}

Зададим матрицу и умножим её на обратную себе же(рис. @fig:016)

![Задание 6](image/16.JPG){#fig:016 width=70%}

При помощи циклов преобразуем матрицы в различные виды(рис. @fig:017)

![Задание 7](image/17.JPG){#fig:017 width=70%}

![Задание 7](image/18.JPG){#fig:018 width=70%}

![Задание 7](image/19.JPG){#fig:019 width=70%}

Создадим функцию эквивалентную одноименной функции из языка R(рис. @fig:020)

![Задания 8](image/20.JPG){#fig:020 width=70%}

![Задания 8](image/21.JPG){#fig:021 width=70%}

Решим линейное уравнение в матричном виде в задании 9(рис. @fig:022)

![Задания 9](image/22.JPG){#fig:022 width=70%}

В 10 задании произведем анализ количества элементов матрицы, удовлетворяющих необходимым условиям(рис. @fig:012)

![Задание 10](image/23.JPG){#fig:023 width=70%}

В задании 10 найдем значения двух сумм(рис. @fig:012)

![Задание 11](image/24.JPG){#fig:024 width=70%}

# Выводы

В результате выполнения данной лабораторной работы были освоены  циклы, функции и сторонние для Julia пакеты для решения задач линейной алгебры и работы с матрицами.

# Список литературы{.unnumbered}

::: {#refs}
:::

