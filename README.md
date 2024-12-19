# Трекер полезных привычек

Проект, помогающий приобретать новые полезные привычки. Создавайте привычку и получайте уведомление о ней в телеграм.


## Требования к проекту

* Python
* Django
* DRF
* PostgreSQL
* Redis
* Celery


## Инструкции по установке и запуску проекта

01. Клонировать репозиторий: `git clone https://github.com/kuzinnatra/courswork_7.git`
02. Перейти в папку проекта: `cd project`
03. Установить зависимости: `pip install -r requirements.txt`
04. Создать файл `.env` в корневой папке проекта и заполнить его по шаблону `.env.sample`.
05. Создать базу данных: `python manage.py migrate`
06. Установить Redis, запустить командой: `redis-server`
07. Запустить сервер: `python manage.py runserver`
08. В программе Postman: зарегистрироваться в админке и создайть привычки
09. В терминале запустить celery worker командой: `celery -A config worker -l INFO`
10. В другом терминале запустить celery beat командой: `celery -A config beat -l info -S django`
11. Зайти в телеграм бот и нажать `START`


## Документация API

Документация API доступна после запуска сервера по адресу: `http://localhost:8000/redoc/` или `http://localhost:8000/docs/`






