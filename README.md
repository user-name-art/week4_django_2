# Пульт охраны банка

Это внутренний репозиторий для сотрудников банка "Сияние". Если вы попали в этот репозиторий случайно, то вы не сможете его запустить, поскольку у вас нет доступа к БД. Однако можно свободно использовать код верстки или посмотреть, как реализованы запросы к БД.

### Как установить
Вам понадобится файл **.env** с настройками. В качестве примера смотрите файл **.env.template**.

* **DB_URL** адрес базы данных
* **DB_ENGINE** движок для доступа к базе данных.
* **DB_PORT** порт для доступа к БД
* **DB_NAME** имя БД
* **DB_USER** имя пользователя для доступа к БД
* **DB_PASSWORD** пароль базы данных.
* **SECRET_KEY** серетный ключ для криптографической подписи.
* **DEBUG_MODE** включить (**True**) или выключить (**False**) режим отладки.
* **ALLOWED_HOSTS** содержит список хостов, на которых может работать текущий сайт. По умолчанию используется **['127.0.0.1', 'localhost']**.

Создайте виртуальное окружение, если это необходимо. Например:
```
python -m venv .venv
```

Python3 должен быть уже установлен. 
Затем используйте `pip` (или `pip3`, есть конфликт с Python2) для установки зависимостей:
```
pip install -r requirements.txt
```
### Как запустить
Выполните в консоли
```
python manage.py runserver 0.0.0.0:8000
```

### Цель проекта

Код написан в образовательных целях на онлайн-курсе для веб-разработчиков [dvmn.org](https://dvmn.org/).
