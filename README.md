# Kittygram

### Разработчик проекта: Лоскутова Татьяна (Loskutova Tatiana)

### Назначение проекта
Данный проект представляет web-приложение для загрузки фотографий котиков, своих или чужих. Основная цель проекта - это автоматический деплой на удаленный сервер.

### Технологический стек
- Python - основной язык программирования.
- Django - фреймворк для разработки веб-приложений.
- Django REST framework - инструмент для создания веб-API на основе Django.
- GIT - система контроля версий проекта
- Pytest - инструмент для тестирования проекта
- Docker - инструмент для запуска приложений в контейнерах.
- Docker compose - нструмент для запуска многоконтейнерных Docker приложений.
- GitHub Actions - автоматизированные рабочие процессы на GitHub для сборки, тестирования и развертывания кода

### Как запустить проект:
- https://tanishaloskut.zapto.org - доменное имя проекта. По этой ссылке доступен в сети интернет.

### Как зполнять данные в .env:

POSTGRES_DB = название базы данных
POSTGRES_USER = имя пользователя БД
POSTGRES_PASSWORD = пароль пользователя БД
DB_NAME= назавние таблицы в бд
DB_HOST= адрес, по которому Django будет соединяться с базой данных. При работе нескольких контейнеров в сети Docker network вместо адреса указывают имя контейнера, где запущен сервер БД
DB_PORT= порт, по которому Django будет обращаться к базе данных. 5432 — это порт по умолчанию для PostgreSQL

### Локальный запуск проекта:

**1)** Клонировать репозиторий и перейти в него в командной строке:

    git clone https://github.com/TatianaLoskutova/kittygram_final

**2)** Cоздать и активировать виртуальное окружение:

    python -m venv venv

    venv/Scripts/activate

**3)** Установить зависимости из файла requirements.txt:

    python -m pip install --upgrade pip

    pip install -r requirements.txt

**4)** Выполнить миграции:

    python manage.py migrate

**5)** Запустить проект:

    python manage.py runserver

![Workflow Status](https://img.shields.io/github/workflow/status/tatianaloskutova/kittygram_final/message check)