# recipe-app-api

Recipe DRF project.

### Running the docker containers

```shell
docker-compose up
```

<br />

### Stoppiing the docker containers

```shell
docker-compose down
```

<br />

### Running flake8 Linting

```shell
docker-compose run --rm app sh -c "flake8"
```

<br />

### Running Django tests

```shell
docker-compose run --rm app sh -c "python manage.py test”
```

<br />

### Starting a project

```shell
docker-compose run --rm app sh -c "django-admin startproject app .”
```

<br />

### To start an new app with example name 'core'

```shell
docker-compose run --rm app sh -c "python manage.py startapp core”
```

<br />

## Helpful Docker Commands

### List all docker volumes

```shell
docker volume ls
```

<br />

### Delete dangling images

```shell
docker rmi $(docker images -f "dangling=true" -q)
```

<br />

### Remove a docker volume

```shell
docker volume rm <volume-name>
```

Example:

```shell
docker volume rm recipe-app-api_dev-db-data
```

<br />
