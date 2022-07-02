**Hello world!**

```



git init	Инициализация репозитория
git add <file>	Добавление файлов под версионный контроль
    git add .	Добавление всех файлов по версионный контроль
git commit	Фиксация изменений
git commit -a -m «comment»	Игнорирование индексации
git commit —amend	Изменение последнего коммита
    git clone <remote>	Клонирование удаленного репозитория
git clone <remote> <dir>	Клонирование удаленного репозитория в указанный каталог
git status	Определение состояния файлов
git diff	Просмотр изменных, но не проиндексированных файлов
git diff —staged	Просмотр проиндексированных файлов, которые войдут в следующий коммит
git rm <file>	Удаление файла с индексацией
git rm —cached <file>	Удаление файла из индекса (при этом файл остается в рабочем каталоге)
git mv <old file> <new file>	Перемещение файлов
git log	Просмотр истории коммитов
git reset HEAD <file>	Отмена индексации файла
git checkout — <file>	Отмена изменений файла
```
##Работа с ветками
git branch	Показ существующих веток
git branch <branch>	Создание новой ветки
git branch -d <branch>	Удаление ветки
git branch -v	Просмотр последнего коммита на каждой из веток
git branch —merged	Просмотр веток, для которых выполнено слияние
git branch —no-merged	Просмотр веток, для которых не выполнено слияние
git branch -D <branch>	Принудительное удаление ветки
git branch —track <branch> <remote branch>	Создание новой ветки из ветки на удаленном сервере
git checkout <branch>	Переход на ветку
git checkout -b <branch>	Создание ветки с переходом на нее
git merge <branch>	Слияние веток
git mergetool	Запуск графического инструмента для разрешения конфликтов
git push <remote> <branch>	Отправка ветки на удаленный сервер
git push <remote> :<branch>	Удаление ветки на удалённом сервере
```
##Работа с удаленным репозиторием
git remote	Отображение удаленных репозиториев
git remote add <alias> <remote>	Добавление удалённых репозиториев
git remote show <remote>	Информация об удаленном репозитории
git remote rename <old name> <new name>	Переименовывание удаленных репозиториев
git remote rm <remote>	Удаление удаленных репозиториев
git fetch <remote>	Получение данных из удаленных репозиториев
git pull <remote> <branch>	Получение данных из удаленного репозитория и слияние с локальным
git push <remote> <branch>	Отправление локальных изменений на удаленный сервер
```
##Конфигурирование
git config --global user.name "Firstname Lastname" — имя пользователя
git config --global user.email mail@example.com — email пользователя
git config --global core.editor emacs — выбор редактора
git config --global merge.tool vimdiff — утилита сравнения
git config --global status.showUntrackedFiles all — пофайловое отображение изменений
git config alias.<alias> <command> — создание псевдонимов для команд
git config --list — проверка настроек
git help <command> — подсказка по команде