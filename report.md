---
# Front matter
lang: ru-RU
title: "Отчёт по лабораторной работе №1"
subtitle: "Дисциплина: математическое моделирование"
author: "Радикорский Павел Михайлович"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
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

Обучение работе с git и markdown

# Задание

Выполнить задания, приведённые в файле git.pdf и сделать отчёт в формате markdown


# Выполнение лабораторной работы

1.1 Подготовка
1.1.1 Установка имени и электронной почты
1.1.2 Параметры установки окончаний строк
1.1.3 Установка отображения unicode

1.2 Создание проекта
1.2.1 Создание страницы «Hello, World»
1.2.2 Создание репозитория
1.2.3 Добавление файла в репозиторий
1.2.4 Проверка состояния репозитория

1.3 Внесение изменений
1.3.1 Измените страницу «Hello, World»

1.4 Индексация изменений
1.4.1 Коммит изменений
1.4.2 Добавление стандартных тегов страницы
1.4.3 История
1.4.4 Получение старых версий
1.4.5 Создание тегов версий
1.4.6 Переключение по имени тега
1.4.7 Просмотр тегов с помощью команды tag

1.5 Отмена локальных изменений (до индексации)
1.5.1 Переключение на ветку master
1.5.2 Изменение hello.html
1.5.3 Проверка состояния

1.6 Отмена проиндексированных изменений (перед коммитом)
1.6.1 Изменение файла и проиндексирование изменения
1.6.2 Проверка состояния
1.6.3 Сброс буферной зоны
1.6.4 Переключение на версию коммита

1.7 Отмена коммитов
1.7.1 Отмена коммитов
1.7.2 Изменение файла и создание коммита
1.7.3 Создание коммита с новыми изменениями, отменяющими предыдущие
1.7.4 Проверка лога

1.8 Удаление коммиттов из ветки
1.8.1 Команда git reset
1.8.2 Проверка истории
1.8.3 Отметка ветки
1.8.4 Сброс коммитов к предшествующим коммиту Oops
1.8.5 Ничего никогда не теряется
1.8.6 Опасность сброса

1.9 Удаление тега oops
1.9.1 Удаление тега oops

1.10 Внесение изменений в коммиты
1.10.1 Изменение страницы, создание коммита
1.10.2 Необходим email
1.10.3 Изменение предыдущего коммита
1.10.4 Просмотр истории

1.11 Перемещение файлов
1.11.1 Переместите файл hello.html в каталог lib

1.12 Второй способ перемещения файлов
1.12.1 Коммит в новый каталог

1.13 Подробнее о структуре
1.13.1 Добавление index.html

1.14 Git внутри: Каталог .git
1.14.1 Каталог .git
1.14.2 База данных объектов
1.14.3 Углубляемся в базу данных объектов
1.14.4 Config File
1.14.5 Ветки и теги
1.14.6 Файл HEAD

1.15 Работа непосредственно с объектами git
1.15.1 Поиск последнего коммита
1.15.2 Вывод последнего коммита с помощью SHA1 хэша
1.15.3 Поиск дерева
1.15.4 Вывод каталога lib
1.15.5 Вывод файла hello.html
1.15.6 Исследуйте самостоятельно

1.16 Создание ветки
1.16.1 Создайте ветку
1.16.2 Добавьте файл стилей style.css
1.16.3 Измените основную страницу
1.16.4 Измените index.html

1.17 Навигация по веткам
1.17.1 Переключение на ветку master
1.17.2 Вернемся к ветке style

1.18 Изменения в ветке master
1.18.1 Создайте файл README в ветке master

1.19 Сделайте коммит изменений README.md в ветку master.
1.19.1 Просмотр отличающихся веток
1.19.2 Просмотрите текущие ветки

1.20 Слияние
1.20.1 Слияние веток

1.21 Создание конфликта
1.21.1 Вернитесь в master и создайте конфликт
1.21.2 Просмотр веток

1.22 Разрешение конфликтов
1.22.1 Слияние master с веткой style
1.22.2 Решение конфликта
1.22.3 Сделайте коммит решения конфликта
1.22.4 Перебазирование как альтернатива слиянию

1.23 Сброс ветки style
1.23.1 Сброс ветки style
1.23.2 Проверьте ветку

1.24 Сброс ветки master
1.24.1 Сброс ветки master

1.25 Перебазирование
1.25.1 Слияние VS перебазирование

1.26 Слияние в ветку master
1.26.1 Слияние style в master
1.26.2 Просмотрите логи

1.27 Клонирование репозиториев
1.27.1 Перейдите в рабочий каталог
1.27.2 Создайте клон репозитория hello

1.28 Просмотр клонированного репозитория
1.28.1 Давайте взглянем на клонированный репозиторий.
1.28.2 Просмотрите историю репозитория
1.28.3 Удаленные ветки

1.29 Что такое origin?

1.30 Удаленные ветки
1.30.1 Список удаленных веток

1.31 Изменение оригинального репозитория
1.31.1 Внесите изменения в оригинальный репозиторий hello
1.31.2 Извлечение изменений
1.31.3 Проверьте README.md

1.32 Слияние извлеченных изменений
1.32.1 Слейте извлеченные изменения в локальную ветку master
1.32.2 Еще раз проверьте файл README.md

1.33 Добавление ветки наблюдения
1.33.1 Добавьте локальную ветку, которая отслеживает удаленную ветку

1.34 Чистые репозитории

1.35 Создайте чистый репозиторий

1.36 Добавление удаленного репозитория

1.37 Отправка изменений

1.38 Извлечение общих изменений

# Выводы

После выполнения данных заданий были получены основы работы с git
