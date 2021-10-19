# Система контроля версий Git и GitHub.

## Что такое git?
Git-это одна из распределенных систем контроля версий.Позволяет управлять версионностью файлов,откатываться до версий,создавать ветки и их сливать.

## Подготовка репозитория.
**Репозиторий**-это хранилище файлов,поддерживающее версионнсть.
Создать репозиторий можно с помощью команды *git init*,примененной в папке с будущим репозиторием.
Для добавление версионности к файлу используется команда *git add <имя файла>*

## Создание "сохранений"
Для создания сохранения необходимо выполнить фиксацию,она же commit.Это можно сделать с помощью команды *git commit* следующим образом:*git commit -m <сообщение>*.Сообщение к коммиту писать **ОБЯЗАТЕЛЬНО**.
Для всех измененных файлов необходимо использовать *git commit* или использовать ключ *-a* при коммите.

## Журнал изменений.

## Перемещения между сохранениями.
Перемещаться на тот или иной коммит нужно с помощью команды *git checkout*.Для этого нужно написать *git checkout <номер коммита из истории>*.Для возврата к самому последнему коммиту надо написать *git checkout <название ветки>*.По умолчанию ветка *master*.
Отменять изменения можно с помощью команд *git revert* и *git reset*.Для этого нужно написать команду *git revert(reset) <номер коммита>*.Команда git revert перейдет к указанному коммиту,создав новый.А git reset перейдет к указанному состоянию и затрет историю изменений.

## Добавление изображений

## Добавление ссылок

## Ветки в git.

## Скачивание удаленного репозитория.