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

Объединить две ветки можно параметром merge с указанием имени ветки. Команда объединит указанную ветку с основной.

git merge existing_branch_name

## Прекращение слияния при конфликте

Прервать слияние в случае конфликта можно параметром merge с флагом --abort.

git merge --abort