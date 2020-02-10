# Using Docker
- Install `docker` and `docker-compose`
- From your project directory, running beneath command:
```
docker-compose up
```
- If you want, you can run composer or artisan through docker. For instance:
```
docker-compose exec php composer install
docker-compose exec php php artisan migrate
docker-compose exec php $YOUR_COMMAND_HERE
```
