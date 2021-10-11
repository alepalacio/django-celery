# Commands:

- pip install django

- pip install celery

- sudo apt-get install rabbitmq-server

- sudo systemctl enable rabbitmq-server

- sudo systemctl start rabbitmq-server

- systemctl status rabbitmq-server

- celery -A <project name> worker -l info

- sudo rabbitmqctl stop

- python manage.py shell

- from <app name>.tasks import add

- add.delay()

- add.apply_async((), countdown=5)