# Инструкция по работе с Git

## Что такое Git?
***Git*** - это одна из реализаций распределенной системы контроля версий, поддерживающие как локальные, так и удалённые репозитории. Самая популярная реализация Git - это [Github](https://github.com)

## Подготовка репозитория
Для создания репозитория используется команда *Git init*. Для этого необходимо открыть в терминале папку с будущим репозиторием и там написать *git init*.

## Создание коммитов

### Создание выполнения коммита
Для того, чтобы выполнить коммит используется команда *git commit*. Для этого в терминале с папкой-репозиторием необходимо написать *git commit -m "<сообщение к коммиту>"*. Сообщение к коммиту писать ***обязательно!!!!***

### Добавление файла к коммиту
Для добавления файла к коммиту используется команда *git add*. Для этого в терминале с папкой-репозиторием необходимо написать *git add <название файла>*.

## Журнал изменений

## Перемещение между коммитами
Для перемещениями между коммитами используется команда checkout. Для этого в терминале с папкой-репозиторием необходимо написать *git checkout <хеш коммита>*. Хеш коммита можно взять из истории коммитов, про которую было рассказано в предыдущем пункте

## Журнал изменений
Для просмотра истории коммитов используется команда *git log*. Для этого в терминале с папкой-репозиторием пишем *git log*. В показанном журнале обязательно будут:
* Хеш (номер) коммита
* дата и время коммита
* Автор коммита
* Текст сообщения к коммиту

## Ветки в Git 
Ветки в системе Git используются для того, чтобы несколько сотрудников (программистов) могли вести работу над одним проектом вместе, или одновременно не машая друг другу. Также ветки можно использать в качестве экспериментов новых функций, при этом не нанеся вред основному проекту.

### Создание новых веток в Git. 
Для того, чтобы создать новую ветку в Git необходимо использовать команду **git branch (поставить пробел после слова branch и написать название ветки **ОБЯЗЯТЕЛЬНО**)**, нажать enter и все, ветка создана. Для того, чтобы убедиться, что ветка создана, используется команда *git branch*, после ее использования в терминале появится список веток, а та, на которой находится пользователь будет подсвечена зеленым и звездочкой.

## Слияние веток и разрешение конфликтов
Слияние веток - это соединение созданных веток с основной (master). При слиянии веток информация из новых веток переносится в master, также если в git что-то идет не по сценарию, тогда возможен конфликт при слиянии веток, который пользователю необходимо разрешить. Для слияния веток используется команда *git merge*, чтобы ей воспользоваться нужно ввести команду git merge addInformation (addInformation в нашем случае просто название ветки, **название может быть любым**) после этой команды произойдет слияние той ветки, на которой находится пользователь, с той, которая дана была в команде git merge.

## Удаление веток
Для того, чтобы удалить ветку в git, необходимо воспользоваться командой **git braches -d**. Когда будет дана команда git brancges -d deleteBranches произойдет удаление ветки с названием deleteBranches (название также абсолютно любое, но понятное и вам, и коллегам).