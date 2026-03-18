---
title: "Лабораторная работа №7"
subtitle: "Создание презентаций с Beamer"
author: "Мохаммадхоссейн Фарзанфар"
institute: "РУДН, Москва"
date: "2026"
theme: "Warsaw"
colortheme: "beaver"
fonttheme: "professionalfonts"
mainfont: "DejaVu Serif"
sansfont: "DejaVu Sans"
monofont: "DejaVu Sans Mono"
header-includes:
  - \usepackage{polyglossia}
  - \setmainlanguage{russian}
  - \setotherlanguage{english}
  - \newfontfamily\russianfont{DejaVu Serif}
  - \newfontfamily\russianfontsf{DejaVu Sans}
  - \newfontfamily\russianfonttt{DejaVu Sans Mono}
---

## Цель работы

Изучение инструментов создания научных презентаций с использованием пакета **Beamer**

- Настройка визуальных тем
- Работа с математическими формулами
- Создание динамических слайдов

---

## Задание

1. Освоить создание презентаций с Beamer
2. Изучить структуру слайдов и блоков
3. Научиться использовать паузы и эффекты
4. Создать постер с Beamerposter

---

## Что такое Beamer?

**Beamer** - это класс LaTeX для создания презентаций

Преимущества:
- Математические формулы высшего качества
- Автоматическая нумерация
- Легкое управление стилями
- Создание PDF с навигацией

---

## Структура презентации

Каждый слайд создается в окружении frame:

`\begin{frame}{Заголовок слайда}`
`Содержание слайда`
`\end{frame}`

### Темы оформления

Стандартные темы Beamer:

- `Warsaw` (используем мы)
- `Madrid`
- `Copenhagen`
- `Frankfurt`
- `Berlin`
- `CambridgeUS`
- `Darmstadt`
- `Dresden`
- `Pittsburgh`
- `Rochester`

Цветовые темы:

- `beaver` (используем мы)
- `crane`
- `dove`
- `seahorse`
- `albatross`
- `beetle`
- `elephant`
- `fly`
- `whale`
- `lily`

## Блоки и колонки

`\begin{block}{Обычный блок}`
`Текст внутри блока`
`\end{block}`

`\begin{alertblock}{Важный блок}`
`Для выделения важной информации`
`\end{alertblock}`

`\begin{examples}`
`Пример использования`
`\end{examples}`


### Математические формулы

Формулы выглядят профессионально:


`E = mc^2`


`\begin{align}`
`\frac{\partial u}{\partial t} &= \alpha \nabla^2 u \\`
`\int_{-\infty}^{\infty} e^{-x^2} dx &= \sqrt{\pi}`
`\end{align}`




## Множества

$$\mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R} \subset \mathbb{C}$$

$$ A \cap B = \emptyset $$

$$ \{ x \in \mathbb{R} : x^2 = 4 \} = \{-2, 2\} $$

## Эффекты появления

Использование `\pause`:

- Первый пункт 
- Второй пункт 
- Третий пункт 


## Beamerposter - создание постеров

Beamerposter - расширение Beamer для создания научных постеров
Особенности:

Поддержка больших форматов (A0, A1)

Масштабирование шрифтов

Многоколоночная верстка

## Структура постера

`\usepackage[orientation=portrait,size=a0,scale=1.4]{beamerposter}`
`\begin{frame}[fragile]`
`\begin{columns}`
`\begin{column}{.33\textwidth}`
`\begin{block}{Заголовок}`
`Текст в первой колонке`
`\end{block}`
`\end{column}`
`\end{columns}`
`\end{frame}`


## Пример кода презентации


`\documentclass{beamer}`
`\usetheme{Warsaw}`
`\usecolortheme{beaver}`
`\usepackage{amsmath}`
`\title{Моя презентация}`
`\author{Мохаммадхоссейн Фарзанфар}`
`\institute{РУДН}`
`\begin{document}`
`\begin{frame}`
`\titlepage`
`\end{frame}`
`\end{document}`



## Пример кода постера

`\documentclass{beamer}`
`\usepackage[orientation=portrait,size=a0]{beamerposter}`
`\title{Научный постер}`
`\author{Мохаммадхоссейн Фарзанфар}`
`\begin{document}`
`\begin{frame}`
`\begin{columns}`
`\begin{column}{.5\textwidth}`
`\begin{block}{Введение}`
`Текст введения...`
`\end{block}`
`\end{column}`
`\end{columns}`
`\end{frame}`
`\end{document}`

## Результаты работы

В ходе работы были созданы:

Презентация из 6 слайдов с темой Warsaw

Постер формата A0 с Beamerposter

Слайды с математическими формулами

Использованы блоки и эффекты появления

## Результаты конвертации (Задача 1)

Результаты экспорта презентации в форматы PDF и Word:

:::::::::::::: {.columns}
::: {.column width="45%"}
![Результат PDF](Result Task1 Pdf.jpg){width=100%}
:::
::: {.column width="45%"}
![Результат Word](Result Task1 Word.jpg){width=100%}
:::
::::::::::::::

## Результаты конвертации (Задача 2)

Результаты экспорта постера в форматы PPTX и Word:

:::::::::::::: {.columns}
::: {.column width="45%"}
![Результат PPTX](Result Task2 pptx.jpg){width=100%}
:::
::: {.column width="45%"}
![Результат Word](Result Task2 word.jpg){width=100%}
:::
::::::::::::::


## Выводы
Beamer позволяет создавать профессиональные презентации

LaTeX обеспечивает высокое качество математических формул

Beamerposter удобен для создания научных постеров

Возможность автоматизации форматирования экономит время

