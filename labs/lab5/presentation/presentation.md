---
## Front matter
lang: ru-RU
title: Лабораторная работа №5
subtitle: Основы информационной безопасности
author:
  - Ищенко Ирина
institute:
  - Российский университет дружбы народов, Москва, Россия


## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Ищенко Ирина Олеговна
  * НПИбд-02-22

:::
::: {.column width="30%"}

:::
::::::::::::::

## Цель работы

Изучение механизмов изменения идентификаторов, применения
SetUID- и Sticky-битов. Получение практических навыков работы в консоли с дополнительными атрибутами. Рассмотрение работы механизма
смены идентификатора процессов пользователей, а также влияние бита
Sticky на запись и удаление файлов.


# Выполнение лабораторной работы

## simpleid.c

![simpleid.c](image/1.png){#fig:001 width=50%}

## Выполнение simpleid

![Выполнение simpleid](image/2.png){#fig:002 width=50%}

## simpleid02

![simpleid02](image/3.png){#fig:003 width=50%}

## simpleid02

![Выполнение simpleid02](image/4.png){#fig:004 width=50%}

## Смена владельца и атрибут

![Смена владельца и атрибут](image/5.png){#fig:005 width=50%}

## readfile.c

![readfile.c](image/6.png){#fig:006 width=70%}

## Изменение владельца и прав

![Изменение владельца и прав](image/7.png){#fig:007 width=70%}

## Отказ в чтении

![Отказ в чтении](image/8.png){#fig:008 width=50%}

## Смена владельца и атрибута

![Смена владельца и атрибута](image/9.png){#fig:009 width=50%}

## Выполнение проверки

![Выполнение проверки](image/10.png){#fig:0010 width=50%}

## Выполнение проверк

![Выполнение проверки](image/11.png){#fig:0011 width=50%}

## Права на файл

![Права на файл](image/12.png){#fig:0012 width=50%}

## Проверка атрибута

![Проверка атрибута](image/13.png){#fig:0013 width=50%}

## Проверка снятия атрибута

![Проверка снятия атрибута](image/14.png){#fig:0014 width=50%}

## Выводы

В ходе лабораторной работы я изучила механизмы изменения идентификаторов, применения
SetUID- и Sticky-битов. Получила практические навыков работы в консоли с дополнительными атрибутами. Рассмотрела работы механизма смены идентификатора процессов пользователей, а также влияние бита Sticky на запись и удаление файлов.
