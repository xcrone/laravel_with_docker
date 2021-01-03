# laravel_with_docker

## Requirement
- Docker
- Docker Compose

## Guide
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

URL
```
http://localhost:8000
```