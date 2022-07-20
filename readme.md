# Инструкция для работы с Git и удалёнными репозиториями

1. один
2. два
3. три
вот получается один из способов создания списков
* а вот другой
* на экране появляются точечки

попробуем сделать заголовки
 основной заголовок выделяется одной #
 # опачки! это же заголовок 1-го уровня! 
 ну а если нужны подзаголовки, то тогда количество решеток становится больше, например две  ##
 ## тадааааамс!
 потом будут уже три ###
 ### ну ты посмотри на этот заголовок!)
 дальше 4 и так далее
 так, с заголовками хватит)
 попробую цитаты, как я посмотрел, они выделяются <>
 <нукась> ну что-то не очень
вот кстати надо пропукать строку, чтобы выглядело все нормально

вооо, другое дело! а теперь выделю я другое дело курсивом, используя ** 

*другое дело!*

 а если использовать по две **, то получится выделение жирным

 **вот**

пробуем ссылки 

[тык сюда и увидешь команды] (https://ru.wikipedia.org/wiki/Markdown)

мне не нравится, а если так 

[давай еще разок] (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

[I'm an inline-style link](https://www.google.com)

кажется надо в [] юзать инглиш

[so](https://www.google.com)

а нет, надо чтобы сразу после [] шли (), без пробелов!

![такс](https://pikabu.ru/story/ui__486408)

попробовал вставить картинку

![noch ein mal](https://pikabu.ru/story/ui__486408)

почему-то в предпросмотре я ее не вижу, но саму команду запомним ставим ! и сразу [] без пробелов

а если так 

![alt text][logo]

[logo]: https://pikabu.ru/story/ui__486408

картинки не видно.. жаль

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| графа 3 is    | сломал | $1600 |
| col 2 is      | а нет, не сломал      |   $12 |
| zebra stripes | огО!      |    $1 |

тут как-то сложна, **надо знать, как выстраивать**

![парась](https://krasivosti.pro/uploads/posts/2021-09/1632394073_6-krasivosti-pro-p-dovolnii-porosenok-zhivotnie-krasivo-foto-6.jpg)

ееееееееееееее! получилось!

так, теперь посмотрел еще одну команду с выделением `текста` работает))

для этого я использовал ``

еще видел, что если юзнуть сразу три ```

``` 
то между ними весь текст будет выделен!
```

ага, красиво и заметно

поизучал создание колонок

итак! для этого используем три дефиса ---
и вот если их юзнуть под текстом, то получится заголовок 1-го уровня
---

так что надо их отделить

нук | даже нашел вертикальную черту на клаве | ооооу ееее
--- | --- | ---
1 | 2 | 3
*name* | **очки** | ~~результат~~


наконец-то, для зачеркивания надо по два ~~

сейчас нашел, как нормально делать цитаты, юзаем только одну >

> вооооооот так вот!

а теперь добавим сюда видео, открываем [] внутри еще одни [] перед вторыми идет ! закрываются вторые [] и сразу, без пробелов (с картинкой ютуба, но что-то не вышло, надо найти логотип ютубчика прост) потом закрывается первая [] и опять без пробелов (а уже тут ссылка на видео)

[![пропустил тут заголовок](https://upload.wikimedia.org/wikipedia/commons/0/09/YouTube_full-color_icon_%282017%29.svg)](https://www.youtube.com/watch?v=FFBTGdEMrQ4)

вооо, нашел логотип и все получилось!

ну вроде как все! по основным командам прошелся


## Команды Git

1. для начала нужно создать репозиторий, т. е. папку, где будет храниться файл

+ для этого используется команда **git init**
 
 2. после мы добавляем нужный файл в git

 + используя команду **git add ./либо указываем имя файла, обязательно с расширением**

3. вообще эти две команды надо использовать почти постоянно, как только была обновлена информация в файле, ну и чтобы git их заполнил и сохранил

забыл указать эти две команды

+ git add

+ а вторая git commit -m 'а здесь комментарий'


так! надо узнать как еще упорядочить то, что сливаешь при конфликте - только вручную или??

4. для создания новой ыетки используется команда 

**git branch а вот тут имя этой ветки**

5. ветки можно слить, т. е. в любую ветку, добавить содержимое другой. я уже сделал это с ветками мастер и 2. для этого необходимо находится в ветке, куда будешь доавлять информацию и указать ветку, откуда ты ее берешь

**git merge а тут названия сливаемой ветки**

6. понравилась еще одна команда, а именно

+ git commit --amend -m 'текст нового коммита'

данная команда позволяет подкорректировать коммит

7. для перемещения между ветками используется команда 

+ git checkout и название ветки

но нам так же показали более классную команду 

+ git checkout -b и название ветки 

таким образом мы создаем новую ветку и сразу перемещаемся в нее

8. сейчас я слил все ветки в одну, а теперь удалю ветки 2, 3 и 4

 + для этого используется команда git branch -d и название ветки

 попробую также удалить сразу 3 ветки


20.07.22

Работа с удаленными репозиториями (с теми, что не на нашем ПК)

тренажер Learn Git Branching

GitHub - сервис, позволяющий хранить свой репозиторий на сервере

git clone - и вставляем ссылку, как на скрине1, но предварительно создаем папку и не делаем ее репозиторием

![screen1](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/d10e7aca-39c3-422c-b0b1-ada70ae46039/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220720%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220720T082038Z&X-Amz-Expires=86400&X-Amz-Signature=886a72fb1b62768df223991b460e2baac941100d13a8e78ed38fbc60d2d7e189&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

cd (change directory) - потом название папки из GitHub

чтобы залить свой репозиторий на GitHub, необходимо для начала создать свой аккаунт там.

![screen2](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/41e7a54e-02c8-4ebc-a1e5-f59e0f880c00/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220720%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220720T082132Z&X-Amz-Expires=86400&X-Amz-Signature=1313a5838d3592447d8eb3c479440ebdd9c315816f238c64f93730c725592729&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

git push - толкать. при первом пуше надо будет авторизоваться

git pull - стянуть, попытается смержить ваш файл с актуальным с GitHub

 вот мы нашли репозиторий, но у нас нет туда доступа, чтобы его загрузить к себе, жмем на Fork (вилка)

 ![screen3](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/93f99adb-ca9b-46f7-874a-043070fa5a46/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220720%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220720T082500Z&X-Amz-Expires=86400&X-Amz-Signature=30710b69f102367fbcbf9edf21af93604e61ba44ac531bdaa4f9f940468a1e1a&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

 на gitHUb принято, чтобы у каждого файла был файл readme, принято называть его капсом (даем описание, что происходит на этом проекте)

получается, мы добавили новую ветку и туда дописали что-то свое, сохранили эти изменения и решили предложить их автору проекта, для этого уже на самом гитхабе появится кнопка Compare & pull request
![screen4](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/69ff4a0e-118e-4a5a-97c2-e0749a4500c8/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220720%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220720T091219Z&X-Amz-Expires=86400&X-Amz-Signature=488a492c9cfd1e3785ba2c5b7566852cb51be7f414b4391888298c2ebca8e462&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

github предложит добавить описание

![screen5](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/a9e6f642-71af-4d64-95e4-c8fad7949eac/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220720%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220720T091314Z&X-Amz-Expires=86400&X-Amz-Signature=095cb25267296195e79eeeb0d8a71c4a21b65732ffd0e3752ac9d68ebb7f08cc&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

Сейчас я добавляю информацию напрямую из GitHub

