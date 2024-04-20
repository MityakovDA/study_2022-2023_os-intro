---
## Front matter
title: "Отчёт по лабораторной работе №10"
author: "Дмитрий Алексеевич Митяков"

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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором Emacs.

# Выполнение лабораторной работы

Открываю emacs
(рис. @fig:001).
![1](image/Снимок экрана от 2024-04-20 22-16-08.png){#fig:001 width=70%}
Создал файл lab07.sh с помощью комбинации Ctrl-x Ctrl-f и набрал текст из задания
(рис. @fig:002).
![2](image/Снимок экрана от 2024-04-20 22-24-01.png){#fig:002 width=70%}
Вырезал одной командой целую строку (С-k).
Вставил эту строку в конец файла (C-y).
Выделил область текста (C-space).
(рис. @fig:004).
![4](image/Снимок экрана от 2024-04-20 22-30-12.png){#fig:004 width=70%}
Скопировал область в буфер обмена (M-w) и вставил область в конец файла (C-y).
(рис. @fig:005).
![5](image/Снимок экрана от 2024-04-20 22-30-26.png){#fig:005 width=70%}
Вновь выделил эту область и на этот раз вырезал её (C-w)затем отменил последнее действие (C-/).
(рис. @fig:006).
![6](image/Снимок экрана от 2024-04-20 22-30-41.png){#fig:006 width=70%}
Научился использовать команды по перемещению курсора.
Переместил курсор в начало строки (C-a).
Переместил курсор в конец строки (C-e).
Переместил курсор в начало буфера (M-<).
Переместил курсор в конец буфера (M->).
(рис. @fig:007).
![7](image/Снимок экрана от 2024-04-20 22-30-51.png){#fig:007 width=70%}
(рис. @fig:008).
![8](image/Снимок экрана от 2024-04-20 22-30-54.png){#fig:008 width=70%}
(рис. @fig:009).
![9](image/Снимок экрана от 2024-04-20 22-30-59.png){#fig:009 width=70%}
(рис. @fig:010).
![10](image/Снимок экрана от 2024-04-20 22-31-20.png)1{#fig:010 width=70%}
(рис. @fig:011).
![11](image/Снимок экрана от 2024-04-20 22-31-26.png){#fig:011 width=70%}
(рис. @fig:012).
Вывел список активных буферов на экран (C-x C-b).
![12](image/Снимок экрана от 2024-04-20 22-32-00.png){#fig:012 width=70%}
Переместился во вновь открытое окно (C-x) o со списком открытых буферов
и переключился на другой буфер и закрыл это окно (C-x 0).
(рис. @fig:013).
![13](image/Снимок экрана от 2024-04-20 22-32-30.png){#fig:013 width=70%}
Поделил фрейм на 4 части: разделил фрейм на два окна по вертикали (C-x 3),
а затем каждое из этих окон на две части по горизонтали (C-x 2)
(рис. @fig:014).
![14](image/Снимок экрана от 2024-04-20 22-33-16.png){#fig:014 width=70%}
Переключился в режим поиска (C-s) и найшел несколько слов, присутствующих
в тексте
(рис. @fig:015).
![15](image/Снимок экрана от 2024-04-20 22-39-03.png){#fig:015 width=70%}
Переключился между результатами поиска, нажимая C-s, а после вышел из режима поиска, нажав C-g.
(рис. @fig:016).
![16](image/Снимок экрана от 2024-04-20 22-39-45.png){#fig:016 width=70%}

# Контрольные вопросы

1. Кратко охарактеризуйте редактор emacs.
-Экранный редактор текста, позволяющий в одном окне редактировать сразу множество файлов
2. Какие особенности данного редактора могут сделать его сложным для освоения новичком?
-Большое количество комбинация клавиш, отличных от привычных
3. Своими словами опишите, что такое буфер и окно в терминологии emacs’а.
-Буфер - место хранения временной информации, окно - визуализация буфера
4. Можно ли открыть больше 10 буферов в одном окне?
-Да
5. Какие буферы создаются по умолчанию при запуске emacs?
-GNU Emacs, scratch, Messages, Quail, Completions
6. Какие клавиши вы нажмёте, чтобы ввести следующую комбинацию C-c | и C-c C-|?
- Сtrl+c, Shift+ и Ctrl+c Ctrl+
7. Как поделить текущее окно на две части?
- C-x 3 или C-x 2.
8. В каком файле хранятся настройки редактора emacs?
- ~/.emacs.
9. Какую функцию выполняет клавиша <-- и можно ли её переназначить?
- Перемещение курсора
10. Какой редактор вам показался удобнее в работе vi или emacs? Поясните почему
- Редактор emacs позволяет работать сразу с несколькими файлами, однако стоит отметить, что в vi комбинации клавиш мне показались более удобными.

# Выводы

Я познакомился с операционной системой Linux. Получил практические навыки работы с редактором Emacs.

# Список литературы{.unnumbered}

::: {#refs}
:::
