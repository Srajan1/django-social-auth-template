How to setup the template:
    docker compose up --build

Everytime a change is made in database

    docker compose exec web python manage.py makemigrations
    docker compose exec web python manage.py migrate

Creating super user
Make sure the initial migrations are applied
    docker exec -it django-docker python manage.py createsuperuser
