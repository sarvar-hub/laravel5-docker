cd {path_project}

sudo docker-compose up -d

(enter app docker-container bash)

composer install
php artisan key:generate
php artisan migrate