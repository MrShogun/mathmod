---
## Front matter
title: "Лабораторная работа №3"
subtitle: "Математическое моделирование"
author: "Николаев Дмитрий Иванович"

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



# Задание

Вариант 29

Между страной Х и страной У идет война. Численность состава войск исчисляется от начала войны, и являются временными функциями x(t) и y(t). В начальный момент времени страна Х имеет армию численностью 202000 человек, а в распоряжении страны У армия численностью в 92000 человек. Для упрощения модели считаем, что коэффициенты a, b, c, h
постоянны. Также считаем P(t) и Q(t) непрерывные функции.
Постройте графики изменения численности войск армии Х и армии У для следующих случаев:

1. Модель боевых действий между регулярными войсками
$$
\frac{dx}{dt} = -0.13x(t) - 0.51y(t) + 0.5\sin (t + 13)
$$
$$
\frac{dy}{dt} = -0.41x(t) - 0.15y(t) + 0.5\cos (t + 2)
$$
2. Модель ведение боевых действий с участием регулярных войск и партизанских отрядов:
$$
\frac{dx}{dt} = -0.08x(t) - 0.76y(t) + \sin (2t) + 1
$$
$$
\frac{dy}{dt} = -0.64x(t)y(t) - 0.07y(t) + \cos (3t) + 1
$$

# Теоретическое введение



# Выполнение лабораторной работы

## Постановка задачи



## Реализация на Julia

Код на Julia:

```julia
using Plots
using DifferentialEquations

```

## Реализация на OpenModelica

Код на OpenModelica:

```OpenModelica

```

## Полученные графики

![Первый случай](image/lab03_1.png){#fig:001 width=70%}

![Второй случай](image/lab03_2.png){#fig:002 width=70%}

# Выводы



# Список литературы{.unnumbered}

::: {#refs}
::: [@lab3]
