---
## Front matter
title: "Отчёт по Внешнему Курсу - Этап 3"
subtitle: "Основы информационной безопасности"
author: "Чистов Даниил Максимович"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 1
lof: true # List of figures
lot: false # List of tables
fontsize: 11pt
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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Пройти внешний курс - Этап 3

# Выполнение лабораторной работы

В лекционных материалах было сказано, что в протоколы прикладного уровня включён HTTPS (рис. [-@fig:001]).

![Задание 001](image/IMG_001.jpg){#fig:001 width=70%}

Обе стороны имеют публичный ключ и секретный ключ, одна сторона открывает публичный ключ, а другая использует его для шифрования, но только владелец секретного ключа его расшифровывает (рис. [-@fig:002]).

![Задание 002](image/IMG_002.jpg){#fig:002 width=70%}

Всё подходит, но очевидно, что хэш-функция не обеспечивает конфиденциальность (рис. [-@fig:003]).

![Задание 003](image/IMG_003.jpg){#fig:003 width=70%}

Первые два ответа - никак не относятся к цифровой подписи, это алгоритм симметричного шифрования (AES) и хэш-функция (рис. [-@fig:004]).

![Задание 004](image/IMG_004.jpg){#fig:004 width=70%}

Т.к. обе стороны по сути проверяются по одному ключу, следовательно это симметричная криптография (рис. [-@fig:005]).

![Задание 005](image/IMG_005.jpg){#fig:005 width=70%}

Асимметричный, т.к. у каждой стороны и свой секретная и открытая часть, и он устанавливает ключ, но не шифрует (рис. [-@fig:006]).

![Задание 006](image/IMG_006.jpg){#fig:006 width=70%}

Т.к. для подписей используется асимметричная криптография, следовательно это публичный протокол (рис. [-@fig:007]).

![Задание 007](image/IMG_007.jpg){#fig:007 width=70%}

Открытый ключ используется для расшифровки подписи, подпись это зашифрованный хэш, ну и сам хэш (рис. [-@fig:008]).

![Задание 008](image/IMG_008.jpg){#fig:008 width=70%}

Конфиденциальность не обеспечивается, т.к. сообщение не шифруется (рис. [-@fig:009]).

![Задание 009](image/IMG_009.jpg){#fig:009 width=70%}

Она создаётся с использование сертифицированных средств криптозащиты, а также имеет юридическую силу, что важно при работе с государством (рис. [-@fig:010]).

![Задание 010](image/IMG_017.jpg){#fig:010 width=70%}

Такие центры именно для этого и созданы, когда речь идёт о безопасности - это наилучший вариант, чем позволять выдавать сертификаты каждой желающей организации (рис. [-@fig:011]).

![Задание 011](image/IMG_010.jpg){#fig:011 width=70%}

SecurePay не считается, т.к. это электронная платёжная система, по сути и Bitcoin по этому не считается (рис. [-@fig:012]).

![Задание 012](image/IMG_011.jpg){#fig:012 width=70%}

Капча лишь может предотвратить (и то не всегда) автоматизированную атаку, а PIN-код + пароль тоже можно подобрать и не нужно иметь доступ к чему-нибудь стороннему (например, телефону) (рис. [-@fig:013]).

![Задание 013](image/IMG_012.jpg){#fig:013 width=70%}

Банк-эмитент - тот, кто выпустил карту, следовательно он несёт ответственность за аутентификацию пользователя, также используется многофакторная аутентификация - что-то, что знает пользователь + что-то, что этот пользователь имеет (телефон) (рис. [-@fig:014]).

![Задание 014](image/IMG_013.jpg){#fig:014 width=70%}

При нахождении потребуется очень много вычислений, переборов - оттого и сложность, однако проверка результата будет быстрой (рис. [-@fig:015]).

![Задание 015](image/IMG_014.jpg){#fig:015 width=70%}

Подходят все варианты (рис. [-@fig:016]).

![Задание 016](image/IMG_015.jpg){#fig:016 width=70%}

Курс успешно пройден (рис. [-@fig:017]).

![Курс успешно пройден](image/IMG_016.jpg){#fig:017 width=70%}


# Выводы

Этап 3 пройден успешно на максимальный балл.

# Список литературы

[Курс "Основы Кибербезопасности" на платформе Stepik](https://stepik.org/course/111511)

