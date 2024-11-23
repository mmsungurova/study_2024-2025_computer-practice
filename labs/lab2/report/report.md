---
## Front matter
title: "Компьютерный практикум по статистическому анализу данных"
subtitle: "Лабораторная работа № 2. Julia. Структуры данных"
author: "Сунгурова Мариян"

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

Основная цель работы -- изучить несколько структур данных, реализованных в Julia, научиться применять их и операции над ними для решения задач.

**Задачи**

1. Используя Jupyter Lab, повторите примеры из раздела 2.2.
2. Выполните задания для самостоятельной работы (раздел 2.4).

# Теоретическое введение

Julia — высокоуровневый свободный язык программирования с динамической типизацией, созданный для математических вычислений.[@julialang]. Эффективен также и для написания программ общего назначения. Синтаксис языка схож с синтаксисом других математических языков, однако имеет некоторые существенные отличия.

Для выполнения заданий была использована официальная документация Julia[@juliadoc].

# Выполнение лабораторной работы

Рассмотрим несколько структур данных, реализованных в Julia.

Несколько функций (методов), общих для всех структур данных:

– isempty() — проверяет, пуста ли структура данных;

– length() — возвращает длину структуры данных;

– in() — проверяет принадлежность элемента к структуре;

– unique() — возвращает коллекцию уникальных элементов структуры,

– reduce() — свёртывает структуру данных в соответствии с заданным бинарным оператором;

– maximum() (или minimum()) — возвращает наибольший (или наименьший) результат вызова функции для каждого элемента структуры данных.

Выполним примеры из лабораторной работы для действий над кортежами(рис. @fig:001 - @fig:002 )

![Примеры. Кортежи](image/1.JPG){#fig:001 width=70%}

![Примеры. Кортежи](image/2.JPG){#fig:002 width=70%}

Также со словарями(рис. @fig:003 - @fig:004)

![Примеры. Словари](image/3.JPG){#fig:003 width=70%}

![Примеры. Словари](image/4.JPG){#fig:004 width=70%}

Рассмотрим также примеры опреций над множествами(рис. @fig:005 - @fig:006)

![Примеры. Множества](image/5.JPG){#fig:005 width=70%}

![Примеры. Множества](image/6.JPG){#fig:006 width=70%}

И с массивами(рис. @fig:007 - @fig:011)

![Примеры. Массивы](image/7.JPG){#fig:007 width=70%}

![Примеры. Массивы](image/8.JPG){#fig:008 width=70%}

![Примеры. Массивы](image/9.JPG){#fig:009 width=70%}

![Примеры. Массивы](image/10.JPG){#fig:010 width=70%}

![Примеры. Массивы](image/11.JPG){#fig:011 width=70%}

![Примеры. Массивы](image/12.JPG){#fig:012 width=70%}

![Примеры. Массивы](image/13.JPG){#fig:013 width=70%}


Выполним задания для самостоятельной работы. С

1. Даны множества: 𝐴 = {0, 3, 4, 9}, 𝐵 = {1, 3, 4, 7}, 𝐶 = {0, 1, 2, 4, 7, 8, 9}. 
Найдем 𝑃 = 𝐴 ∩ 𝐵 ∪ 𝐴 ∩ 𝐵 ∪ 𝐴 ∩ 𝐶 ∪ 𝐵 ∩ 𝐶.(рис. @fig:014)

![Задание 1](image/14.JPG){#fig:014 width=70%}

2. Приведем свои примеры с выполнением операций над множествами элементов
разных типов. (рис. @fig:016 - @fig:017)

![Задание 2](image/15.JPG){#fig:015 width=70%}

![Задание 2](image/16.JPG){#fig:016 width=70%}

![Задание 2](image/17.JPG){#fig:017 width=70%}


1. Создадим разными способами массивы и вектора. Для создания нужных массивов, используем генераторы и циклы(рис. @fig:018 - @fig:023)

![Задание 3](image/18.JPG){#fig:018 width=70%}

![Задание 3](image/19.JPG){#fig:019 width=70%}

![Задание 3](image/20.JPG){#fig:020 width=70%}

![Задание 3](image/21.JPG){#fig:021 width=70%}

![Задание 3](image/22.JPG){#fig:022 width=70%}

![Задание 3](image/23.JPG){#fig:023 width=70%}


4. Создадим массив squares, в котором будут храниться квадраты всех целых чисел от 1
до 100.(рис. @fig:024 )

![Задание 4](image/24.JPG){#fig:024 width=70%}

5. Подключим пакет Primes (функции для вычисления простых чисел). Затем сгенерируем массив myprimes, в котором будут храниться первые 168 простых чисел. 
Определим также 89-е наименьшее простое число и срез массива с 89-го до 99-го элемента включительно, содержащий наименьшие простые числа.(рис. @fig:025)

![Задание 5](image/25.JPG){#fig:025 width=70%}

6. Вычислим выражения(рис. @fig:026 )

   ![Задание 6](image/26.JPG){#fig:026 width=70%}

# Выводы

В результате выполнения данной лабораторной работы были изучены структуры данных, реализованных в Julia: словарь, массив, кортеж множество, также юыли получены практические навыки применения этих структур и операций над ними решения задач.

# Список литературы{.unnumbered}

::: {#refs}
:::

