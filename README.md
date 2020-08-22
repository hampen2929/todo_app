# Docker

```
docker-compose build
docker-compose up
docker exec -it react_develop_1 /bin/sh
```

# React

```
mkdir react

cd react
npx create-react-app . --template redux
```

```
sudo chown yuya:yuya /home/yuya/workspace/api_tasks/ -R
```

```
npm install axios
```

```
npm start
```

# Django

```
docker build -t django_image ./

docker run -it \
--rm \
--name django \
-v $HOME/workspace/api_tasks/:/usr/src/app/ \
-p 8000:8000 \
django_image \
/bin/bash

docker exec -it django /bin/bash

```

```
mkdir django
cd django
python -m django startproject api_tasks .
python -m django startapp api
```

```
python manage.py runserver 0.0.0.0:8000
```

```
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser

```
