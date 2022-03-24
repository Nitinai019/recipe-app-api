# recipe-app-api
Recipe app api source code.


# build docker
`
docker build .
`
# build docker-compose when components has update.
`
docker-compose build
`
# create create django project using docker
`
docker-compose run app sh -c "django-admin.py startproject app ."
`
# run django and flake8 test

`
docker-compose run app sh -c "python manage.py test && flake8"
`

# create django app

`
docker-compose run app sh -c "python manage.py startapp core"

`

# make migrations
`
docker-compose run app sh -c "python manage.py makemigrations core"
`