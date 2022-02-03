copy env file
cd {path_project}

sudo docker-compose up -d
(enter app docker-container bash)
sudo docker exec -it app bash
composer install
php artisan key:generate
php artisan migrate