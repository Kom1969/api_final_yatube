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
Создание публикации
```
POST http://127.0.0.1:8000/api/v1/posts/
```
Удаление публикации
```
DELETE http://127.0.0.1:8000/api/v1/posts/{id}/
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
Подписки
```
GET http://127.0.0.1:8000/api/v1/follow/
```
Подписка
```
POST http://127.0.0.1:8000/api/v1/follow/
```
Получить JWT-токен
```
POST http://127.0.0.1:8000/api/v1/jwt/create/
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
