# Learning Log

Django-приложение: темы и записи, у каждого пользователя свои. Регистрация, вход, выход.

## Локально

    python -m venv ll_env && ll_env\Scripts\activate   (Linux: source ll_env/bin/activate)
    pip install -r requirements.txt
    python manage.py migrate
    python manage.py createsuperuser
    python manage.py runserver

## Сервер (Docker Compose)

Скопируйте `.env.example` в `.env`, подставьте ключ, адрес и порт, затем `docker compose up -d --build`.
Администратор: `docker compose exec web python manage.py createsuperuser`.
