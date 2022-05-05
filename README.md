This is an educational repository that contains homeworks, completed as part of Vadim Ksendzov's training course on software testing. 
Here I am learning how to work in GitHub. 
Below is my homework and solution

# XML
### Создать внешний репозиторий c названием XML.
`
https://github.com/demiurgusnen9/XML.git
`
### Клонировать репозиторий XML на локальный компьютер.
```
$ git clone https://github.com/demiurgusnen9/XML.git
 
 Cloning into 'XML'...
 remote: Enumerating objects: 3, done.
 remote: Counting objects: 100% (3/3), done.
 remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
 Receiving objects: 100% (3/3), done.
```
### Внутри локального XML создать файл “new.xml”.
```
$ cd XML
$ touch new.xml
```
### Добавить файл под гит.
`
$ git add new.xml
`
### Закоммитить файл.
```
$ git commit -m "add new.xml"
 
 [main e7881ba] add new.xml
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.xml
``` 
### Отправить файл на внешний GitHub репозиторий.
```
$ git push
 
 Enumerating objects: 4, done.
 Counting objects: 100% (4/4), done.
 Delta compression using up to 2 threads
 Compressing objects: 100% (2/2), done.
 Writing objects: 100% (3/3), 275 bytes | 275.00 KiB/s, done.
 Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
 To https://github.com/demiurgusnen9/XML.git
 596d53f..e7881ba  main -> main
```
### Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.
```
$ vim new.xml
 <xml>
        <фио> Masalskaya Alena Viktorovna </фио>
        <возраст>30</возраст>
        <количество домашних животных>1</количество домашних животных>
        <будущая желаемая зарплата>500$</будущая желаемая зарплата>
 </xml>
 ```
### Отправить изменения на внешний репозиторий.
```
$ git commit -am "add info in new.xml"

 warning: LF will be replaced by CRLF in new.xml.
 The file will have its original line endings in your working directory
 [main aa2534b] add info in new.xml
 1 file changed, 6 insertions(+)

$ git push

 Enumerating objects: 5, done.
 Counting objects: 100% (5/5), done.
 Delta compression using up to 2 threads
 Compressing objects: 100% (3/3), done.
 Writing objects: 100% (3/3), 457 bytes | 457.00 KiB/s, done.
 Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
 To https://github.com/demiurgusnen9/XML.git
 e7881ba..aa2534b  main -> main
```
### Создать файл preferences.xml
`
$ touch preferences.xml
`
### В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, страна которую хотели бы посетить) в формате XML.
```
$ vim preferences.xml

 <xml>
        <Любимый фильм>Трудности перевода</Любимый фильм>
        <Любимый сериал>Клиника</Любимый сериал>
        <Любимая еда>Кукурузные_палочки </Любимая еда>
        <Любимое время года>Зима</Любимое время года>
        <Страна которую хотели бы посетить>Исландия</Страна которую хотели бы посетить>
 </xml>
```
### Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML
```
$ vim skills.xml

 <xml>
        <skills1>Базовая теория (Что такое тестирование, багрепорты, документация, виды, методы, направления тестирования и т.п.) SDLC, STLC</skills1>
        <skills2>Что такое клиент-серверная архитектура</skills>
        <skills3> HTTP Методы запросов на сервер</skills3>
        <skills4>Коды ответов HTTP сервера</skills4>
        <skills5>Структуры HTTP запросов и ответов</skills5>
        <skills6>Что такое JSON, XML. Их структура</skills6>
        <skills7>Тестирование API через Postman (JS, автотесты API)</skills7>
        <skills8>Снятие и чтение логов c внешнего сервера</skills8>
        <skills9>Снифинг http web трафика через Charles и Fiddler</skills9>
        <skills10>Dev Tools веб браузеров (Google Chrome, FireFox)</skills10>
        <skills11>VPN. (Как работает, зачем нужен, как использовать, варианты инструментов)</skills11>
        <skills12>Мобильное тестирование</skills12>
        <skills13>Особенность iOS, Android, гайдлайны<skills13>
        <skills14>Сборка iOS приложений на XCode</skills14>
        <skills15>Сборка Android приложений на Android Studio</skills15>
        <skills16>ADB (управление андройд девайсами)</skills16>
        <skills17>Настройка прокси и vpn на iOS и Android</skills17>
        <skills18>Перехват (сниффинг) мобильного трафика через Charles и Fiddler на iOS и Android</skills18>
        <skills19>Командная строка (terminal) Linux (копирование, создание, просмотр, перемещение файлов на серверах без графического интерфейса)</skills19>
        <skills20>Основы bash скриптинг, автоматизация рутинных задач на сервере</skills20>
        <skills21>Доступ к удалённым серверам</skills21>
        <skills22>Основы SQL (Create, Delete, Drop, Insert Into, Select, From, Where, Join)</skills22>
        <skills23>База данных Postgres (установка, настройка и использование)</skills23>
        <skills24>Нереляционная база данных Redis (установка, настройка и использование)</skills24>
        <skills25>Нагрузочное тестирование в Jmeter</skills25>
        <skills26>Методология разработки Scrum</skills26>
        <skills27>Python. (Изучение основ. Создание клиент серверного приложения)</skills27>
 </xml>
```
### Сделать коммит в одну строку.
```
 $ git add . && git commit -m "add preferences.xml and skills.xml with info"
 
 [main 3fd28e1] add preferences.xml and skills.xml with info
 2 files changed, 36 insertions(+)
 create mode 100644 preferences.xml
 create mode 100644 skills.xml
```
### Отправить сразу 2 файла на внешний репозиторий.
```
$ git push
 
 Enumerating objects: 5, done.
 Counting objects: 100% (5/5), done.
 Delta compression using up to 2 threads
 Compressing objects: 100% (4/4), done.
 Writing objects: 100% (4/4), 1.74 KiB | 1.74 MiB/s, done.
 Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
 To https://github.com/demiurgusnen9/XML.git
 aa2534b..3fd28e1  main -> main
```
### На веб интерфейсе создать файл bug_report.xml.
`
done
`
### Сделать Commit changes (сохранить) изменения на веб интерфейсе.
`
done
`
### На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.
```
<bug_report>
<ID>ID</ID>
<Summary>Короткое описание</Summary>
<Steps to Reproduce>Шаги воспроизведения</Steps to Reproduce>
<Expected Result>Ожидаемый результат</Expected Result>
<Actual Result>Фактический результат</Actual Result>
<Severity>Серьезность</Severity>
</bug_report>
```
### Сделать Commit changes (сохранить) изменения на веб интерфейсе.
`
done
`
### Синхронизировать внешний и локальный репозиторий XML
```
$ git pull
 
 remote: Enumerating objects: 7, done.
 remote: Counting objects: 100% (7/7), done.
 remote: Compressing objects: 100% (5/5), done.
 remote: Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
 Unpacking objects: 100% (6/6), 1.47 KiB | 68.00 KiB/s, done.
 From https://github.com/demiurgusnen9/XML
 3fd28e1..23cd44f  main       -> origin/main
 Updating 3fd28e1..23cd44f
 Fast-forward
 bug_report.xml | 8 ++++++++
 1 file changed, 8 insertions(+)
 create mode 100644 bug_report.xml
```
