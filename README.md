# WWS_Test
Using for WWS test

git clone https://github.com/laravel/laravel.git wwsapp
cd ~/wwsapp
docker run --rm -v $(pwd):/app composer install
# sudo chown -R $USER:$USER ~/laravel-app


docker-compose up -d 
# docker-compose up --build --force-recreate --no-deps -d app


docker-compose exec app php artisan key:generate
docker-compose exec app php artisan config:cache

docker-compose exec db bash