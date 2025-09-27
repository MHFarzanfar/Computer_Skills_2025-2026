---
# Front matter
lang: ru-RU
title: "Лабораторная работа №2"
subtitle: "Дисциплина: Компьютерный практикум по научному письму"
author: "Мохаммадхоссейн Фарзанфар"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # Список рисунков
lot: true # Список таблиц
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Познакомиться со структурой LaTeX-документа и созданием простых документов, изучить основные команды и специальные символы LaTeX.

# Задание

1. Изучить структуру LaTeX-документа

2. Создать простой документ с базовыми элементами

3. Освоить основные команды и окружения LaTeX

4. Изучить работу со специальными символами


# Выполнение лабораторной работы

1. Изучение структуры LaTeX-документа
Изучил базовую структуру LaTeX-документа, которая состоит из:

Преамбулы (настройки документа)

Тела документа (содержимое)

2. Создание простого документа
Создал файл document.tex со следующим содержимым:

![Исходный код LaTeX-документа](image02/image_01.jpg){ width=50% }



3) Компиляция документа

Выполнил компиляцию командой:

pdflatex document.tex

4) Добавление базовых элементов

Добавил в документ базовые элементы:
 Разделы и подразделы (`\section`, `\subsection`)
 Специальные символы с экранированием
 Сноски (`\footnote`)
 Неразрывные пробелы (`~`)

Все элементы работают корректно после компиляции.


# Пример добавления изображений

![Компиляция документа с помощью pdflatex](image02/image_02.jpg){ width=70% }

![Результат компиляции в PDF-формате](image02/image_03.jpg){ width=70% }



# Выводы

В ходе лабораторной работы №2 была изучена структура LaTeX-документа и освоены основные принципы создания документов. Были выполнены следующие задачи:

Изучена базовая структура LaTeX-документа (преамбула и тело)

Создан простой LaTeX-документ с разделами и подразделами

Освоена компиляция документа с помощью pdflatex

Изучена работа со специальными символами LaTeX

Практически применены знания о форматировании текста