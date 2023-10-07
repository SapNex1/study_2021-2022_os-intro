---
## Front matter
title: "Отчёт по лабораторной работе №3. Введение в работу с Octave."
subtitle: "Предмет: научное программирование"
author: "Александр Сергеевич Баклашов"

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

Изучить основы Octave

# Теоретическое введение

GNU Octave — свободная программная система для математических вычислений, использующая совместимый с MATLAB язык высокого уровня.

Предоставляет интерактивный командный интерфейс для решения линейных и нелинейных математических задач, а также проведения других численных экспериментов. Кроме того, Octave можно использовать для пакетной обработки. Язык Octave оперирует арифметикой вещественных и комплексных скаляров, векторов и матриц, имеет расширения для решения линейных алгебраических задач, нахождения корней систем нелинейных алгебраических уравнений, работы с полиномами, решения различных дифференциальных уравнений, интегрирования систем дифференциальных и дифференциально-алгебраических уравнений первого порядка, интегрирования функций на конечных и бесконечных интервалах. Этот список можно легко расширить, используя язык Octave (или используя динамически загружаемые модули, созданные на Си, C++, Фортране и других). [1]

# Выполнение лабораторной работы

## Простейшие операции

1. Выполним простейшие операции в Octave (рис. [-@fig:001])

![Простейшие операции](image/1.png){ #fig:001 width=80% }

## Операции с векторами

2. Выполним операции с векторами в Octave (рис. [-@fig:002])

![Операции с векторами](image/2.png){ #fig:002 width=90% }

## Вычисление проектора

3. Выполним вычисление проектора в Octave (рис. [-@fig:003])

![Вычисление проектора](image/3.png){ #fig:003 width=90% }

## Матричные операции

4. Выполним матричные операции в Octave (рис. [-@fig:004])

![Матричные операции](image/4.png){ #fig:004 width=70% }

## Построение простейших графиков

5. Построим график функции $sinx$ на интервале $[0, 2π]$. (рис. [-@fig:005])

![График функции](image/5.png){ #fig:005 width=90% }

## Улучшение графика

6.  Улучшим построенный график (рис. [-@fig:006])

![Улучшенный график](image/6.png){ #fig:006 width=90% }

## Два графика на одном чертеже

7. Нарисуем два графика на одном чертеже (рис. [-@fig:007])

![Два графика на одном чертеже](image/7.png){ #fig:007 width=90% }

## График $𝑦 = 𝑥^2 sinx$

8. Построим график $𝑦 = 𝑥^2 sinx$ (рис. [-@fig:008])

![График](image/8.png){ #fig:008 width=90% }

## Сравнение циклов и операций с векторами

9. Вычислим сумму с помощью цикла. Создадим файл loop_for.m (рис. [-@fig:009])

![loop_for](image/9.png){ #fig:009 width=90% }

10. Вычислим сумму с помощью операций с векторами. Создадим файл loop_vec.m (рис. [-@fig:010])

![loop_vec](image/10.png){ #fig:010 width=90% }

11. Запустим оба файла и сравним их производительность (рис. [-@fig:011])

![Запуск кода](image/11.png){ #fig:011 width=90% }

# Вывод

В ходе данной лабораторной работы я изучил основы программной среды Octave.

# Библиография

1. Лабораторная работа №3. Введение в работу с Octave. - 9 с. [Электронный ресурс]. М. URL: [Лабораторная работа №3. Введение в работу с Octave.](https://esystem.rudn.ru/pluginfile.php/2089335/mod_resource/content/3/003-octave-intro.pdf) (Дата обращения: 20.09.2023).