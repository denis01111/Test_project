# Инструкции по командам в git и Markdown

## Основные команды в git
+ git init - иницизализируем папку, то есть добавляем репозиторий (хранилище)
+ git add fileName (название файла) - добавляем файл в git, чтобы его отслеживать
+ git status - проверяем что у нас происходит в git
+ ctrl + s -сохраняем изменения
+ git commit -m “Комменатрий об изменениях” - помещяем/сохраняем с комменатриями
+ git diff - просмотр разницы между сохраненным и текущим файлом
+ git log - просмотр изменений в ветках
+ git branch - список веток, *Зеленым - отмечается ветка в которой мы находимся
+ git branch branchName - создание новой ветки
+ git branch -d branchName - удаление ветки
+ git merge branchName - добавление ветки в текущюgitю ветку, в которой находимся
+ git checkout branchName - перключение между ветками
+ git log —graph - выводит все ветки в виде графов
+ git push - отправка файлов в удаленный репозиторий
+ git pull - вытягивание файлов из ***нашего репозитория*** с последующим слиянием
+ git clone - клонирование/вытягивание файлов из ***чужого репозитория***

Порядок действия такой:
1. Делаем fork к себе чужого репозитория
2. Создаем папку локальную, куда будем выгружать файлы
3. Делаем git init пустой папки
4. Делаем в эту папку git pull
5. Создаем новую ветку, в которой будем работать

# Работа в Markdown

### Выделение текста 

*Выделение курсивом обрамляется знаком звездочкой с двух сторон или нижнее подчеркивание*. Например:

*Курсив* или _Курсив_

**Выделение полужирными обрамляется двумя звездочками с двух сторон или двумя нижними подчеркиваниями**. Например:

**Курсив** или __Курсив__

_Текст может быть курсивом и **полужирными**_

***Полужирный и курсив тремя звездчкоами с двух сторон***

### Списки

Нумерованный 1. или Ненумерованный * или + (с отступом)

1. Текст 1
    * Подтекст A
    * Подтекст Б
    * Подтекст C

2. Текст 2
* Текст 1
* Текст 2
+ Текст 1
+ Текст 2

### Работа с изображениями
Чтобы добавить изображение, изображением добавляем в папку с файлом md.
Текст начинается с воскл. знака, далее квадратные скобки для текст, в случае если изображение не отобразиться и далее круглые скобки, куда необходимо вставить название файла с расширением. Например:

![GB](/Image.JPG)
![Book](/python.PNG)

Изображение, как правило, сохраняют отдельно. Создаем файл .gitignore и добавляем туда файл картинку с расширением. Далее git add .ignore и после этого комитим наш основной файл

### Ссылки

Для просмотра ссылок используем круглые скобки для ссылки. Например:

Команды для MD (https://docs.microsoft.com/ru-ru/contribute/how-to-write-links)

Чтобы длинные URL не затрудняли чтение и написание документа Markdown, есть вариант присвоения каждой ссылке определенных ID (меток/переменных). Можно сделать это несколькими способами:

Ссылаемся на [cсылку][geekbrains] через ID. Объявляем метку позже по аналогии со сносками. Цифрами обозначить тоже можно: [Google][1], [Yandex][2]

Еще можно так встраивать ссылки: [geekbrains]

[geekbrains]: https://gb.ru/ "GeekBrains"

[1]: https://www.google.com/ (Сайт Google)

[2]: https://yandex.ru/ (Сайт Яндекса)

[geekbrains]: https://gb.ru/

### Цитаты

> Выделение текста для цитирования, нужно добавление впереди знака ">"

### Таблицы

| Виды аналитиков | Зарплата, руб. | Ссылка | Работадатель |
| -----|------|------| --|
| Бизнес аналитик | от 150 000 | [ссылка]("https://hh.ru/vacancy/66782383?from=vacancy_search_list&hhtmFrom=vacancy_search_list&query=%D0%91%D0%B8%D0%B7%D0%BD%D0%B5%D1%81%20%D0%B0%D0%BD%D0%B0%D0%BB%D0%B8%D1%82%D0%B8%D0%BA")| ![HH](/HH.PNG)|
| Аналитик данных | от 130 000 |[ссылка]("https://hh.ru/vacancy/66681320?query=%D0%B0%D0%BD%D0%B0%D0%BB%D0%B8%D1%82%D0%B8%D0%BA%20%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85&from=vacancy_search_catalog&hhtmFrom=vacancy_search_catalog") | ![HH](/HH.PNG)|
| Финансовый аналитик | от 100 000 |[ссылка]("https://hh.ru/vacancy/67259061?from=vacancy_search_list&hhtmFrom=vacancy_search_list&query=%D1%84%D0%B8%D0%BD%D0%B0%D0%BD%D1%81%D0%BE%D0%B2%D1%8B%D1%85%20%D0%B0%D0%BD%D0%B0%D0%BB%D0%B8%D1%82%D0%B8%D0%BA") | ![HH](/HH.PNG)|
| Системный аналитик |от 200 000|[ссылка]("https://hh.ru/vacancy/67227770?query=%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%BD%D1%8B%D0%B9%20%D0%B0%D0%BD%D0%B0%D0%BB%D0%B8%D1%82%D0%B8%D0%BA&from=vacancy_search_catalog&hhtmFrom=vacancy_search_catalog") | ![HH](/HH.PNG)|
|Веб-аналитик|от 120 000|[ссылка]("https://hh.ru/vacancy/66782990?from=vacancy_search_list&hhtmFrom=vacancy_search_list&query=%D0%92%D0%B5%D0%B1%20%D0%B0%D0%BD%D0%B0%D0%BB%D0%B8%D1%82%D0%B8%D0%BA") | ![HH](/HH.PNG)|
|Аналитик 1С|от 100 000|[ссылка]("https://hh.ru/vacancy/67296754?from=vacancy_search_list&hhtmFrom=vacancy_search_list&query=%D0%B0%D0%BD%D0%B0%D0%BB%D0%B8%D1%82%D0%B8%D0%BA%201%D1%81") | ![HH](/HH.PNG)|
|Продуктовый аналитик|от 150 000|[ссылка]("https://hh.ru/vacancy/67174418?query=%D0%BF%D1%80%D0%BE%D0%B4%D1%83%D0%BA%D1%82%D0%BE%D0%B2%D1%8B%D0%B9%20%D0%B0%D0%BD%D0%B0%D0%BB%D0%B8%D1%82%D0%B8%D0%BA&from=vacancy_search_catalog&hhtmFrom=vacancy_search_catalog") |![HH](/HH.PNG)|
|Аналитик BI|от 175 000|[ссылка]("https://hh.ru/employer/534148?hhtmFrom=vacancy_search_catalog") | ![HH](/HH.PNG)|

### Код
Код на Python:

```

x = int(input())

if x > 0:

    print(x)

else:

    print(-x)

```
