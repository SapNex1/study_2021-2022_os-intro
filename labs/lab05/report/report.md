---
## Front matter
title: "Отчёт по лабораторной работе №5. Подгонка полиномиальной кривой и матричные преобразования в Octave."
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

Изучить способы подгонки полиномиальной кривой и некоторые матричные преобразования в Octave

# Теоретическое введение

GNU Octave — свободная программная система для математических вычислений, использующая совместимый с MATLAB язык высокого уровня.

Предоставляет интерактивный командный интерфейс для решения линейных и нелинейных математических задач, а также проведения других численных экспериментов. Кроме того, Octave можно использовать для пакетной обработки. Язык Octave оперирует арифметикой вещественных и комплексных скаляров, векторов и матриц, имеет расширения для решения линейных алгебраических задач, нахождения корней систем нелинейных алгебраических уравнений, работы с полиномами, решения различных дифференциальных уравнений, интегрирования систем дифференциальных и дифференциально-алгебраических уравнений первого порядка, интегрирования функций на конечных и бесконечных интервалах. Этот список можно легко расширить, используя язык Octave (или используя динамически загружаемые модули, созданные на Си, C++, Фортране и других). [1]

# Выполнение лабораторной работы

## Подгонка полиномиальной кривой

1. Построим график точек, под которые будем подгонять параболу (рис. [-@fig:001])

![График точек](image/1.png){ #fig:001 width=80% }

2. В статистике часто рассматривается проблема подгонки прямой линии к набору данных. Решим более общую проблему подгонки полинома к множеству точек. Пусть нам нужно найти параболу по методу наименьших квадратов для набора точек, заданных матрицей выше. (рис. [-@fig:002])

![Парабола](image/2.png){ #fig:002 width=90% }

## Polyfit

3. Процесс подгонки может быть автоматизирован встроенными функциями Octave. Для этого мы можем использовать встроенную функцию для подгонки полинома polyfit. (рис. [-@fig:003])

![Polyfit](image/3.png){ #fig:003 width=90% }

## Матричные преобразования

4. Представим изображение домика в виде матрицы. (рис. [-@fig:004])

![Матричные преобразования](image/4.png){ #fig:004 width=70% }

## Вращение

5. Повернём граф дома на 90 и 225 градусов. (рис. [-@fig:005])

![Вращение](image/5.png){ #fig:005 width=90% }

## Отражение

6.  Отразим граф дома относительно прямой $𝑦 = 𝑥$. (рис. [-@fig:006])

![Отражение](image/6.png){ #fig:006 width=90% }

## Дилатация

7. Увеличим граф дома в 2 раза (рис. [-@fig:007])

![Дилатация](image/7.png){ #fig:007 width=90% }

# Вывод

В ходе данной лабораторной работы я изучил способы подгонки полиномиальной кривой и некоторые матричные преобразования в Octave.

# Библиография

1. Лабораторная работа №5. - 10 с. [Электронный ресурс]. М. URL: [Лабораторная работа №5.](https://esystem.rudn.ru/pluginfile.php/2089339/mod_resource/content/2/README.pdf) (Дата обращения: 05.10.2023).