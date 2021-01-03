# Laravel with Docker

## Requirement
- Docker
- Docker Compose

<br>

## Configuration
Setup environment file
```
cp .env.example .ev
```

Make sure to change database host in .env file
```
DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=database
DB_USERNAME=database
DB_PASSWORD=database123
```

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

Generate key
```
docker-compose exec php php artisan key:generate
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