# Avito Analytics Academy
[AAA lecture on working with the docker](https://avito-analytics-academy.ru/)

## Step 1. Build
```bash
docker build -t=app:0.0.1 .
docker images
```

## Step 2. Run
```bash
curl localhost:8080
docker run --rm -d -p 8080:8080 --name=flask_app app:0.0.1
curl localhost:8080
docker stop flask_app
```

## Step 3. Push
```bash
docker tag app:0.0.1 <INSERT_YOUR_DOCKER_HUB_ACC>/app:0.0.1
docker push <INSERT_YOUR_DOCKER_HUB_ACC>/app:0.0.1
```

## Step 4. Pull
```bash
docker run --rm -d -p 8080:8080 --name=flask_app <INSERT_YOUR_DOCKER_HUB_ACC>/app:0.0.1
curl localhost:8080
docker stop flask_app
```

