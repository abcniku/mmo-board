# Использовано в проекте
- фреймворк Django
- регистриция через allauth
- Celery
- Redis

# Установка и запуск

Клонировать репозиторий:
`git clone https://github.com/abcniku/mmoboard.git`

Создать и войти в вирутальное окружение

Установить необходимые библиотеки:
1) `pip install django`
2) `pip install django-bootstrap4`
3) `pip install django-allauth`
4) `pip install celery`
5) `pip install redis`
6) `pip install -U "celery[redis]"`

Установить и запустить сервер Redis

Запустить Celery
`celery -A MMORPG_board worker -l INFO -B`

Сделать миграции
`python manage.py makemigrations`
`python manage.py migrate`

Запустить Django сервер
`python manage.py runserver`
