# recipe-app-api
Recipe app api source code.


# build docker
docker build .

# build docker-compose
docker-compose build

# create create django project using docker

docker-compose run app sh -c "django-admin.py startproject app ."

# settup trivis ci

