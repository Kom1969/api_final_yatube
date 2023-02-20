# Проект «API для Yatube»
## Социальная сеть блогеров
### Описание
Этот проект создан для общения блогеров со всего мира.
### Технологии
Python 3.9
Django 2.2.19
### Запуск проекта в dev-режиме
- Установите и активируйте виртуальное окружение
- Установите зависимости из файла requirements.txt
```
pip install -r requirements.txt
``` 
- В папке с файлом manage.py выполните команду:
```
python3 manage.py runserver
```
### После запуска проекта, документация будет доступна по адресу:
```
http://localhost:port/redoc/
```
### Примеры
Получение публикаций
```
GET http://127.0.0.1:8000/api/v1/posts/
```
```
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
Создание публикации
```
POST http://127.0.0.1:8000/api/v1/posts/
```
```
{
"text": "string",
"image": "string",
"group": 0
}
```
Удаление публикации
```
DELETE http://127.0.0.1:8000/api/v1/posts/{id}/
```
```
{
  "detail": "Учетные данные не были предоставлены."
}
```
Получение комментариев
```
GET http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/
```
Добавление комментария
```
POST http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/
```
Удаление комментария
```
DELETE http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/{id}/
```
Информация о сообществе
```
GET http://127.0.0.1:8000/api/v1/groups/{id}/
```
```
{
  "id": 0,
  "title": "string",
  "slug": "string",
   "description": "string"
}
```
Получить JWT-токен
```
POST http://127.0.0.1:8000/api/v1/jwt/create/
```
```
{
  "username": "string",
  "password": "string"
}
```
Обновить JWT-токен
```
POST http://127.0.0.1:8000/api/v1/jwt/refresh/
```
Проверить JWT-токен
```
POST http://127.0.0.1:8000/api/v1/jwt/verify/
```

### Автор
Михаил
```
https://github.com/Kom1969
```
