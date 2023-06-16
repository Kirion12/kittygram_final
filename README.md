# Социальная сеть любителей котов Kittygram

### URL
https://kittygramsd.myftp.org/

### Описание
Интерактивный сайт с личным кабинетом с возможностями публикации фотографий котов.

### Технологии
Python 3.11
Django 4.1,
Django REST framework, 
React

### Запуск проекта в dev-режиме
- Клонируйте репозиторий и перейдите в него в командной строке:
```
git clone https://github.com/kirion12/kittygram_final.git
```
```
cd kittygram_final
```
- Запустите проект с помощью команды:
```
docker compose up
```
- Соберите статику Django с помощью команды:
```
docker compose exec backend python manage.py collectstatic
```
- Скопируйте статику командой:
```
docker compose exec backend cp -r /app/collected_static/. /static/static/
```