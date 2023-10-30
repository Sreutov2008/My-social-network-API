Инструкция по запуску API проекта Yatube (v1) (Яндекс.Практикум) 
=====

Описание проекта
----------
Проект создан в рамках учебного курса Яндекс.Практикум.

API сервис для [проекта социальной сети Yatube](https://github.com/Sreutov2008/hw05_final.git). 

Реализован REST API CRUD для основных моделей проекта, для аутентификации примненяются JWT-токены. 
В проекте реализованы ограничения доступа, фильтрации, сортировки и поиск по запросам пользователей, реализована пагинация ответов от API, установлено ограничение количества запросов к API. 

Системные требования
----------
* Python 3.7+
* Works on Linux, Windows, macOS, BSD

Стек технологий
----------
* Python 3.7
* Django 3.2 
* Django Rest Framework
* Pytest
* PyJWT
* SQLite3

Установка проекта из репозитория (Windows)
----------

1. Клонировать репозиторий и перейти в него в командной строке:
```bash
git clone https://github.com/Sreutov2008/hw05_final.git

cd API_FINAL_YATUBE
```
2. Cоздать и активировать виртуальное окружение:
```bash
python -m venv env

source env/bin/activate
```
3. Установить зависимости из файла ```requirements.txt```:
```bash
python -m pip install --upgrade pip

pip install -r requirements.txt
```
4. Выполнить миграции:
```bash
cd yatube_api

python manage.py migrate
```
5. Запустить проект (в режиме сервера Django):
```bash
python manage.py runserver
```
Документация к проекту
----------
Документация API после установки и запуска доступна по адресу ```http://127.0.0.1:8000/redoc/```.
