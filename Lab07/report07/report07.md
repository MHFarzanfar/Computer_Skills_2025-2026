---
# Front matter
lang: ru-RU
title: "Лабораторная работа №7"
author: "Мохаммадхоссейн Фарзанфар"
# Formatting
pdf-engine: lualatex
header-includes:
  - \usepackage{polyglossia}
  - \setmainlanguage{russian}
  - \setotherlanguage{english}
  - \newfontfamily\russianfont{DejaVu Serif}
  - \newfontfamily\russianfontsf{DejaVu Sans}
  - \newfontfamily\russianfonttt{DejaVu Sans Mono}
  - \setmainfont{DejaVu Serif}
  - \setsansfont{DejaVu Sans}
  - \setmonofont{DejaVu Sans Mono}
  - \usepackage{graphicx}
  - \usepackage{caption}
  - \usepackage{pdfpages}
# Bibliography settings
bibliography: bib/references.bib
citeproc: true
reference-section-title: Библиография
nocite: |
  @*
---
\newpage

# Цель работы

Изучение инструментов создания научных презентаций с использованием пакета **Beamer** и научных постеров с помощью **Beamerposter**. Настройка визуальных тем, работа с математическими формулами и автоматизация отчета.

\newpage

# 2 Задание

1.  Освоить создание презентаций с использованием класса Beamer
2.  Изучить структуру презентаций, создание слайдов и управление контентом
3.  Научиться использовать паузы и эффекты появления для динамических презентаций

\newpage

# Выполнение работы

## 1. Создание презентации (Beamer)

В ходе работы была создана презентация на тему "Introduction to LaTeX". Я использовал тему `Warsaw` и цветовую схему `beaver`. 

### Основные элементы презентации:
- Использование блоков (`block`) для выделения ключевых идей.
- Написание математических формул (производные, множества).
- Применение эффектов перехода (`\pause`, `\uncover`).

\newpage

![Логотип университета и оформление](logo.jpg){ width=70% }

*(Здесь можно вставить скриншоты ваших слайдов)*

![Слайд с математическими формулами](Compile Presentation 1.png){ width=70% }

\newpage

## 2. Создание научного постера (Beamerposter)

Был разработан постер формата A0. Основная сложность заключалась в правильном распределении контента по колонкам.

### Структура постера:
- Три колонки (`columns`) для текста и графики.
- Использование больших шрифтов (`\VeryHuge`, `\Large`).
- Внедрение кода и математических примеров.

![Внешний вид готового постера](Compile Poster 1.png){ width=70% }

\newpage

---

# Исходный код (Source Code)

Ниже приведены полные тексты исходных файлов.

## Полный код презентации (presentation.tex)

![Результат конвертации постера в PPTX](Result Task2 pptx.jpg){ width=70% }

![Результат конвертации постера в Word](Result Task2 word.jpg){ width=70% }


```
\documentclass{beamer}
\usetheme{Warsaw}
\usecolortheme{beaver}
\usepackage{amsmath}
\usepackage{graphicx}
\author{Mohammadhossein Farzanfar}
\title{A Brief Introduction to LaTeX for Scientific Writing}
\institute{RUDN University}
\begin{document}
\begin{frame}
\titlepage
\end{frame}
\begin{frame}{Main Message: Why Use LaTeX?}
\begin{block}{Key Idea (Covered Early)}
LaTeX is great for scientific documents because it handles math, references, and structure logically.
\pause
Example: Unlike word processors, LaTeX uses markup for sections.
\end{block}
\end{frame}
\begin{frame}{Math in LaTeX}
A \alert{set} is a collection of objects.
\[ Z = \{\text{cow}, \text{pig}, \text{elephant}\}. \]
\begin{align*}
\mathbb{N} &= \{1,2,3,\ldots\} \\
\mathbb{Z} &= \{\ldots,-2,-1,0,1,2,\ldots\}
\end{align*}
\end{frame}
\end{document}
```

\newpage

## Полный код постера (poster.tex)

![Результат конвертации презентации в PDF](Result Task1 Pdf.jpg){ width=70% }

![Результат конвертации презентации в Word](Result Task1 Word.jpg){ width=70% }


```
\documentclass[xcolor={svgnames}]{beamer}
\usetheme{Warsaw}
\usecolortheme{beaver}
\usepackage[orientation=portrait,size=a0,scale=1.4]{beamerposter}
\usepackage{graphicx}
\usepackage{amsmath}
\title{A Brief Introduction to LaTeX for Scientific Writing}
\author{Mohammadhossein Farzanfar}
\begin{document}
\begin{frame}[fragile]
\begin{columns}
\begin{column}{1\textwidth}
\centering \VeryHuge A Brief Introduction to LaTeX \\
\Large Mohammadhossein Farzanfar \vspace{1cm}
\end{column}
\end{columns}
\begin{columns}
\begin{column}{.33\textwidth}
\begin{block}{Why LaTeX?}
LaTeX handles complex math better than Word.
\end{block}
\end{column}
\end{columns}
\end{frame}
\end{document}
```

\newpage
# Приложение

## Полная презентация (PDF)
В данном разделе представлена полная версия созданной презентации.

\includepdf[pages={-},scale=0.8,frame]{presentation.pdf}

\newpage
## Научный постер (PDF)
Ниже представлен научный постер, созданный С Beamerposter.

\includepdf[pages={-},fitpaper]{poster.pdf}

\newpage


# Выводы
В ходе работы были освоены пакеты Beamer и Beamerposter. Созданные документы демонстрируют возможности LaTeX в подготовке высококачественных визуальных материалов для научных конференций.

\newpage


