# Commands:

- pip install django

- pip install celery

- sudo apt-get install rabbitmq-server

- sudo systemctl enable rabbitmq-server

- sudo systemctl start rabbitmq-server

- systemctl status rabbitmq-server.service

- sudo rm -rf /var/lib/rabbitmq/mnesia/

- ps auxww | grep rabbit | awk '{print $2}' | sudo xargs kill -9

- sudo service rabbitmq-server start

- celery -A <project name> worker -l info

- celery -A <project name> worker -l info --pool=solo

- celery -A <project name> worker --loglevel=INFO

- sudo rabbitmqctl stop

- python manage.py shell

- from django.core.mail import send_mail

- send_mail("<email title>","<email body>","<email sender>",["<email receiver>"], fail_silently=False)

- from <app name>.tasks import add

- add.delay()

- add.apply_async((), countdown=5)