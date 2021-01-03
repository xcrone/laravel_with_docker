# laravel_with_docker

## Requirement
- Docker
- Docker Compose

<br>

## Start Container
Build container image
```
docker-compose build
```

Start service
```
docker-compose up -d
```

Install package
```
docker-compose exec php composer install
docker-compose exec php npm install
```

Migrate database
```
docker-compose exec php php artisan migrate
```

Run the application tests
```
docker-compose exec php php artisan test
```
<br>

Search this url in browser:
```
http://localhost:8000
```

<br>

## Stop Container
Stop service
``` 
docker-compose stop
```

Kill service
```
docker-compose down
```