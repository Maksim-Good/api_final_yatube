# api_final
api final

## Описание:
API бекэнда для взаимодействия с фронтом. 

## Как запустить проект:
### Cоздать и активировать виртуальное окружение:

py -3.9 -m venv venv
source venv/bin/activate

### Установить зависимости из файла requirements.txt:

python -m pip install --upgrade pip
pip install -r requirements.txt

### Выполнить миграции:

python manage.py migrate

### Запустить проект:

python manage.py runserver

## Документация проекта:

http://127.0.0.1:8000/redoc/

## Примеры запросов:

- POST http://127.0.0.1:8000/api/v1/jwt/create/ - получить JWT-токен
- POST http://127.0.0.1:8000/api/v1/jwt/refresh/ - обновить JWT-токен


- GET http://127.0.0.1:8000/api/v1/posts/ - получить все посты
- POST http://127.0.0.1:8000/api/v1/posts/ - создать пост
- DELETE http://127.0.0.1:8000/api/v1/posts/{id}/ - удалить пост

- GET http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/{id}/ - получить комментарии к посту

- GET http://127.0.0.1:8000/api/v1/follow/ - получить свои подписки

- GET http://127.0.0.1:8000/api/v1/groups/ - получить список групп
- GET http://127.0.0.1:8000/api/v1/groups/{id}/  - получить информацию о группе
