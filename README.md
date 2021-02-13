<br>
<p align="center">
<img src="files/static/logoGit.png" />
<br>
<br>
<a target="_blank" href="https://t.me/devops_mops"><img src="files/static/logoTelegram.png" height="30" /></a>
<a target="_blank" href="https://www.youtube.com/channel/UCqC3c7UHtwoX2wy7fdHc6gg"><img src="files/static/logoYoutube.png" height="30" /></a>
</p>
<br>

# Git - Быстрый старт

## Навигация

- [**Основные команды**](#Основные-команды){:target="_blank"}
- [**Работа с ветками**](#Работа-с-ветками)
- [**Работа с репозиторием**](#Работа-с-репозиторием)
- [**Настройка Git**](#Настройка-Git)

## Основные команды

Создать пустой репозиторий Git в указанном каталоге.
```
git init <directory>
```

При запуске без аргументов текущий каталог будет инициализирован как репозиторий Git.
```
git init
```

Клонировать репозиторий на локальный компьютер через HTTP или SSH.
```
git clone <repo>
```

Поместите все изменения в директории для следующей фиксации.
```
git add <directory>
```

Вместо директории можно указать имя файла
```
git add <file>
```

Все файлы в текущей директории
```
git add .
```

Зафиксировать состояние репозитория
```
git commit -m "<message>"
```

List which files are staged, unstaged, and untracked.
```
git status
```

Display the entire commit history using the default format.
For customization see additional options.
```
git log
```

Show unstaged changes between your index and
working directory.
```
git diff
```

## Работа с ветками
List all of the branches in your repo. Add a <branch> argument to
create a new branch with the name <branch>.
```
git branch
```

Create and check out a new branch named <branch>.
```
git checkout
```

Create and check out a new branch named <branch>.
Drop the -b flag to checkout an existing branch.
```
git checkout -b <branch>
```

Merge <branch> into the current branch.
```
git merge <branch>
```

## Работа с репозиторием

Получите указанную удаленную копию текущей ветки и немедленно объедините ее с локальной копией.
```
git pull <remote>
```

Переместите ветку в <remote> вместе с необходимыми коммитами и
объекты. Создает именованную ветку в удаленном репо, если она не существует.
```
git push
```

## Настройка Git

Указать имя автора, которое будет использоваться для всех коммитов текущим пользователем.
```
git config --global user.name <name>
```

Указать адрес электронной почты автора, который будет использоваться для всех коммитов текущим пользователем.
```
git config --global user.email <email>
```

Открыть файл глобальной конфигурации в текстовом редакторе для редактирования вручную.
```
git config --global --edit
```

Указать текстовый редактор по умолчанию
```
git config --system core.editor <editor>
```