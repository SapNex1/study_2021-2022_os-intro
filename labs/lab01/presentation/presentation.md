---
## Front matter
lang: ru-RU
title: Лабораторная работа №1. Управление версиями.
author: |
	Alexander S. Baklashov
institute: |
	RUDN University, Moscow, Russian Federation

date: 21 September, 2023

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

# Цель работы

– Изучить идеологию и применение средств контроля версий.

– Освоить умения по работе с git.

# Выполнение лабораторной работы

## Установка gh в Fedora Linux

Установим gh в Fedora Linux

![Установка gh](image/1.png){ #fig:001 width=70% }

## Базовая настройка git

Зададим имя и email владельца репозитория

![Имя и email](image/2.png){ #fig:002 width=90% }

Зададим имя начальной ветки, параметр autocrlf, параметр safecrlf.

![Задача параметров](image/3.png){ #fig:003 width=90% }

## Создание ключей ssh

Создадим ключ ssh по алгоритму rsa с ключём размером 4096 бит.

![ssh rsa](image/4.png){ #fig:004 width=90% } 

## Создание ключей ssh

Создадим ключ ssh по алгоритму ed25519

![ssh ed25519](image/5.png){ #fig:005 width=70% }

## Создание ключа GPG

Сгенерируем ключ с определёнными параметрами

![Ключ GPG](image/6.png){ #fig:006 width=50% }

## Добавление GPG ключа в GitHub

Выведем список ключей и копируем отпечаток приватного ключа

![GPG](image/7.png){ #fig:007 width=90% }

## Добавление GPG ключа в GitHub

Cкопируем сгенерированный GPG ключ в буфер обмена

![Копирование GPG](image/8.png){ #fig:008 width=90% }

## Добавление GPG ключа в GitHub

Перейдём в настройки GitHub, нажмём на кнопку New GPG key и вставим полученный ключ в поле ввода.

![Добавление GPG](image/9.png){ #fig:009 width=90% }

## Настройка автоматических подписей коммитов git

Используя введённый email, укажем Git применять его при подписи коммитов

![Подписи](image/10.png){ #fig:010 width=90% }

## Настройка gh

Совершим настройку gh

![gh](image/11.png){ #fig:011 width=90% }

## Шаблон для рабочего пространства

Создадим репозиторий курса на основе шаблона 

![Репозиторий](image/12.png){ #fig:012 width=90% }

## Шаблон для рабочего пространства

Настроим каталог курса

![Каталог](image/13.png){ #fig:013 width=90% }

## Шаблон для рабочего пространства

Отправим файлы на сервер

![Отправка файлов](image/14.png){ #fig:014 width=70% }

# Выводы

В ходе данной лабораторной работы я изучил идеологию и применение средств контроля версий, а также освоил умения по работе с git.