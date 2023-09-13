# Руководство пользователя по работе с Git
## Основные команды c лекции
* git init - инициализирует репозиторий
* git --version - показывает текущую версию Git
* git status - показывает текущее состояние Git и есть ли изменения, которые нужно сохранить
* git add - добавляет содержимое рабочего каталога в индекс для последующего коммита
* tab - автоматическое заполнение данных терминалом
* git commit - зафиксировать/сохранить
* git log - журнал изменений
* git checkout - показывает разницу между текущим файлом и сохраненным
## Команды с семинара
* git clear - очистить терминал
* git config --global user.name "Your name" - Добавить свое имя
* git config --global user.email "Your email" - Добавить свой имейл
* git commit -m "Initial commit" - Добавить комментарий при сохранении
* ctrl + s - сохранение изменений в файле, не в гит
* git commit -a -m "Commit" - Сохранить и добавить комментарий в обход команды git add, удобно при работе с одним файлом или если надо сохранить изменения сразу во всех. В ином случае стоит сначала использовать  git add для определенного файла и затем к этому делать коммит.
* git commit -am "Commit" - Более короткая версия верхней команды
* git commit --amend -m "new com" - Изменить последний оставленный коммит
* git checkout *f501* - Вернуться на сохраненную версию, указав первые 4 символа номера, инициализирующего коммит.
* git checkout master - Вернуться "назад в будущее" к последней сохраненной версии.
## Дополнительная информация
* .md - расширение языка markdown
* U - неотслеживаемый файл
* A - отслеживаемый файл
* Open preview - предпоказ форматирования
* M - модифицирован
* Q - выйти из режима просмотра истории
* HEAD detached at - "оторванная голова" Маркер-предупреждение, о том, что если внести изменения в более старом сохранении, то будут потеряны все последующие. Только создав ветку можно будет вносить изменения.
## Markdown
* **Жирный текст**
* *Курсивный текст*
* ***Жирный курсив***
* ~~Зачёркнутый текст~~
* # Заголовок в начале строки
* ## Заголовок поменьше
* ### И ещё меньше 
* 1. Нумерованные
* 2. списки
* "*" Ненумерованные списки
* * Подсписки без нумерации
* * * Под-под списки без нумерации
* * * * И так далее
## О ветках Git
* git branch - посмотреть список веток
* git branch new_branch_name - создание новой ветки
* git checkout branch_name - переключение на указанную ветку
* git commit -am "Изменения в ветку branch_name"
* git merge branch_name - Слияние веток. Изменения из указанной ветки переходят в ветку, на которой находишься.
* git log --graph - посмотреть дерево коммитов и веток
* git branch -d branch_name - удаление ветки
* git checkout -b branch_name - создает новую ветку и переключается на неё
## О работе с удаленными репозиториями, GitHub
* git clone https://github.com/VoYuva/HW_5023_4991.git - копирует удаленный репозиторий
* git pull - подтягивает изменения из текущего удаленного репозитория и делает merge с нашей локальной версией
* git push - отправляет изменения в нашей локальной версии репозитория в удаленный репозиторий, требует авторизации на внешнем репозитории
* pull request - команда для предложения изменений, запрос на вливание изменений
* fork - "вилка", копия репозитория, сделанная другим человеком, не автором оригинального репозитория и предполагающая изменения
* git branch -m main - переименовывает текущую ветку в main
* git remote add origin https://github.com/VoYuva/HW_5023_4991.git - связывает наш локальный репозиторий с удаленным репозиторием
* git push --set-upstream origin branch_name - посылает изменения в определенной ветке в удаленный репозиторий
## The end