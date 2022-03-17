# Актуально для mobil

## Перед работой нужно очистить глобальные найстройки (config global) git.

### Способ 1 

Перейти в C:\Users\username\

Найти файл .gitconfig

Открыть в текстовом редакторе и удалить поля: user.name, user.email

### Способ 2

Октрыть консоль (win + R -> cmd) или git bash

Прописать

- git config --global user.name ""
- git config --global user.email ""

Далее можно производить работу с git

## Работа с git

1. Инициализировать новый репозиторий git init
2. Настроить git
   1. git config user.name "your name"
   2. git config user.email "your email"

       ***Внимание!** нет атрибута --global*

## push на github

Если при вводе git push -u origin yourbranch появилась ошибка:

> remote: Permission to repo.git denied to someuser.
>
> fatal: unable to access 'https://github.com/repo.git/':  The requested URL returned error: 403

То нужно добавить настройку

git config --global credential.github.com.useHttpPath true

Будет дополняться
