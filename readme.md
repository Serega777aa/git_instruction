## Как задать имя пользователя и адрес электронной почты

git config --global user.name "Tara Routray"
git config --global user.email "dev@tararoutray.com"

## Инициализация репозитория

Создать пустой репозиторий Git или вновь инициализировать существующий можно параметром init. При инициализации он создаст скрытую папку. В ней содержатся все объекты и ссылки, которые Git использует и создаёт в истории работы над проектом.

git init

## Добавление отдельных файлов или всех файлов в область подготовленных файлов

Добавить отдельный файл в область подготовленных файлов можно параметром add с указанием имени файла. Просто замените somefile.js на актуальное имя.

git add somefile.js

Кроме того, можно добавить все файлы и папки в эту область, предоставив wildcard . вместо имени файла:

git add .

## Проверка статуса репозитория

git status

##  Внесение изменений однострочным сообщением

При создании коммита в репозитории можно добавить однострочное сообщение с помощью параметра commit с флагом -m

git commit -m "Your short summary about the commit"

## Просмотр истории коммитов

git log

## Перемещение между коммитами или ветками.

git checkout

## Создание новой ветки и переход в неё

Создать новую ветку можно с помощью параметра branch, указав имя ветки.

## Просмотр списка веток

Можно просматривать полный список веток, используя параметр branch

git branch

## Удаление ветки

Удалить ветку можно параметром branch с добавлением флага -d и указанием имени ветки.
git branch -d existing_branch_name

## Слияние двух веток

git merge existing_branch_name

## Прекращение слияния при конфликте

Чтобы прекратить слияние команда git --abort
Прервать слияние в случае конфликта можно параметром merge с флагом --abort.

git merge --abort

## Добавление удалённого репозитория
Добавить удалённый репозиторий можно параметром remote add, указав shortname и url требуемого репозитория.
git remote add origin https://github.com/someurl..

## Отправка новой ветки в удалённый репозиторий
Передать новую ветку в удалённый репозиторий можно параметром push с флагом -u, указав имя репозитория и имя ветки.

git push -u origin new_branch

## Получение изменений из удалённого репозитория
Для загрузки изменений из удалённого репозитория используется параметр pull. Он скачивает копию текущей ветки с указанного удалённого репозитория и объединяет её с локальной копией.

git pull