# Установка

1. Клонируйте репозиторий
```
https://github.com/YuryYuferev/Internet_shop.git
cd Internet_shop
```

2. Создайте виртуальное окружение и активируйте его
```
python -m venv venv
venv/Scripts/activate
```
3. Установите зависимости
```
pip install -r requirements.txt --upgrade
```

4. Запустите миграции и загрузите данные в БД
```
python manage.py migrate
python manage.py loaddata data.json
```
5. Создайте администратора магазина
```
python manage.py createsuperuser
```
6. Запустите сервер
```
python manage.py runserver
```
7. Откройте браузер и перейдите по адресу http://127.0.0.1:8000/admin/. Введите имя пользователя и пароль 
администратора, чтобы войти в панель управления магазином.
