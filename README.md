# journal-Gazette

This project is a newspaper site developed with the [Django](https://github.com/django/django) framework, utilizing  [PostgreSQL](https://www.postgresql.org/)
database to store data and employing [Docker](https://www.docker.com/)  for simplified deployment and management.

## features

- Secure user registration and login functionality.
- CRUD functionality for articles, with publish, edit, and delete options for article authors.
- Authenticated users can post comments on articles.
- Utilize Django admin app for convenient management of users, articles, and comments.

## Technologies used

- [Python 3.11](https://www.python.org/) , Programming Language.
- [Django 4.0.10](https://docs.djangoproject.com/en/4.2/releases/4.0.10/) , Web Framework.
- [Docker](https://www.docker.com/) , Container Platform.
- [PostgreSQL](https://www.postgresql.org/) , Database.

## run project

Build and run the Docker containers using Docker Compose:

```shell
$ docker-compose up -d 
```

Apply the database migrations:

```shell
$ docker-compose exec web python manage.py migrate 
```

Create a superuser:

```shell
$ docker-compose exec web python manage.py createsuperuser 
```

After these steps, you can access the website by navigating to `http://localhost:8000/` in your web browser.   
and the admin site can be accessed by navigating to `http://localhost:8000/admin/` and entering the superuser
credentials.