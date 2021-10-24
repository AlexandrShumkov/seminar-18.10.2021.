# Система контроля версий Git и ветки.

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
Все изменения и сохранения можно посмотреть с помощью команды *git log*.Для просмотра изменений в графическом ввиде набираем команду *git log --graph*.
До слияния веток,из данной ветки можно наблюдать изменения и сохранения,которые были сделаны только в этой ветке.
## Перемещения между сохранениями.
Перемещаться на тот или иной коммит нужно с помощью команды *git checkout*.Для этого нужно написать *git checkout <номер коммита из истории>*.Для возврата к самому последнему коммиту надо написать *git checkout <название ветки>*.По умолчанию ветка *master*.
Отменять изменения можно с помощью команд *git revert* и *git reset*.Для этого нужно написать команду *git revert(reset) <номер коммита>*.Команда git revert перейдет к указанному коммиту,создав новый.А git reset перейдет к указанному состоянию и затрет историю изменений.

## Добавление изображений
Существует возможность добавлять в текст изображения.Необходимо нужную картинку поместить в рабочую папку и добавить ее в git командой *git add <название файла>*.Затем сделать запись в строку текста.Например:
![monkey](monkey.jpg "Gorillas")
В квадратных скобках указывается текст,который будет видно,если картинка пропадет.В круглых,название файла и коментарий к ней.

## Добавление ссылок
Также можно добавлять в текст ссылки.Нужно ввести в строку текста следующее:
[link](https://img1.fonwall.ru/o/zl/wings-snow-bird-of-prey-owl.jpeg "Летун").
В квадратных скобках само слово *ссылка* или *link*,а в круглых-полностью адрес ссылки и в ковычках коментарий.

## Ветки в git.
В git применяется возможность ветвления.Т.е.работа с файлом в разных направлениях и множеством людей.Есть основная ветка *master*.При создании новой ветки применяется команда *git branch new_branch_name*.При слиянии веток,из ветки куда надо добавить информацию,вызывается команда *git merge <имя ветки,из которой добавляем>*.Когда надо удалить ненужную ветку,используем команду *git branch -d <имя удаляемой ветки>*.


