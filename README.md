# I. Введение в Git
## A. Определение и назначение
1. Git - это распределенная система контроля версий, используемая для отслеживания изменений в файлах и координации работы над этими файлами между несколькими людьми.
2. Она позволяет эффективно сотрудничать, отслеживать изменения и легко откатываться к предыдущим версиям.

## B. Распределенная система контроля версий
1. В отличие от централизованных систем контроля версий, Git не полагается на центральный сервер для хранения всей истории проекта.
2. Каждый пользователь имеет полную копию репозитория, включая его историю, на своей локальной машине.
3. Пользователи могут работать автономно и независимо друг от друга, что делает его подходящим как для небольших, так и для крупных проектов.

# II. Настройка Git
## A. Установка Git
1. Git можно установить на различные операционные системы, такие как Windows, macOS и Linux.
2. Инструкции по установке можно найти на официальном сайте Git.

## B. Настройка Git с помощью информации о пользователе
1. После установки Git должен быть сконфигурирован с информацией о пользователе, такой как имя и адрес электронной почты.
2. Эта информация связана с каждой фиксацией и помогает определить, кто внес изменения.

## C. Инициализация нового хранилища
1. Чтобы начать использовать Git в проекте, необходимо инициализировать репозиторий.
2. Это можно сделать, перейдя в корневой каталог проекта и выполнив команду "git init".
3. Инициализация репозитория создает скрытый каталог ".git", в котором хранятся все необходимые файлы и метаданные Git.

# III. Основные команды Git
## A. git init
1. Инициализирует новый Git-репозиторий в текущем каталоге.

## B. git add
1. Добавляет файлы в область хранения, подготавливая их к фиксации.
2. Файлы могут быть добавлены по отдельности с помощью команды "git add <filename>" или все файлы в текущем каталоге с помощью команды "git add .".

## C. git commit
1. Создает новый коммит с изменениями в области постановки.
2. Коммит представляет собой снимок хранилища в определенный момент времени.
3. Каждый коммит имеет уникальный идентификатор, сообщение о коммите, информацию об авторе и ссылку на родительский(ие) коммит(ы).
4. Команда "git commit -m "Commit message"" используется для создания фиксации с кратким описательным сообщением.

## D. git status
1. Отображает текущее состояние репозитория.
2. Показывает, какие файлы изменены, поставлены или не отслежены.
3. Помогает понять состояние репозитория и какие изменения готовы к фиксации.

## E. git log
1. Показывает историю фиксации репозитория.
2. Журнал включает сообщения о фиксации, авторов, временные метки и идентификаторы фиксации.
3. Команда "git log --oneline" обеспечивает более сжатое представление истории фиксации.
## F. git push
1. Загружает локальные коммиты в удаленный репозиторий, например GitHub.
2. Команда "git push <remote> <branch>" перемещает коммиты из локальной ветки в указанный удаленный репозиторий и ветку.

HEAD -- это голова.
Коммит -- это всему голова.
Статусы файлов:
<тут пустая строка!>

```mermaid
%% описание схемы
```
<и тут пустая строка!>
```mermaid
graph LR;
  untracked -- "git add" --> staged/tracked;
  staged/tracked -- "git commit" --> tracked/comitted;
  staged/tracked -- "Изменения" --> modified/tracked;
  tracked -- "Изменение" --> modified/tracked;
%% стрелка без текста для примера: 
  A --> B;
``` 
