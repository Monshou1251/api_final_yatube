## Yatube API

### Описание проекта:

Yatube project являет собой удобную и компактную социальную сеть для друзей, где каждый может поделиться чем угодно, будь то котики или фотографии с любимыми. Можно делиться своими впечатлениями комментируя посты друзей или даже свои собственные.


### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/kittygram2plus.git
```

```
cd kittygram2plus
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

```
source env/bin/activate
```

```
python3 -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```

## Tech
Yatube API uses a number of open source projects to work properly:

- [Python] - a programming language that lets you work quickly and integrate systems more effectively.
- [Django] - a high-level Python web framework

## Author
Автор сего ваяния - Гриша Юрченко. 
Ссылка на github - https://github.com/Monshou1251/api_final_yatube

## Requests examples
Samples of how this API works could be found through Redoc - http://127.0.0.1:8000/redoc/

GET request:
http://127.0.0.1:8000/api/v1/posts/
```sh
{
  "count": 123,
  "next": "http://api.example.org/accounts/?offset=400&limit=100",
  "previous": "http://api.example.org/accounts/?offset=200&limit=100",
  "results": [
    {
      "id": 0,
      "author": "string",
      "text": "string",
      "pub_date": "2021-10-14T20:41:29.648Z",
      "image": "string",
      "group": 0
    }
  ]
}
```

PUT request:
http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/{id}/
```sh
{
  "text": "string"
}
```
Response samples:
```sh
{
  "id": 0,
  "author": "string",
  "text": "string",
  "created": "2019-08-24T14:15:22Z",
  "post": 0
}
```


