composer create-project laravel/lumen WebServersApi
composer create-project laravel/lumen ApiGateway

cd WebServersApi
cd ApiGateway

php -S localhost:8003 -t public
php -S localhost:8008 -t public

php artisan make:migration CreateWebServersTable --create=webservers

php artisan migrate - to create database tables

php artisan db:seed

(php artisan migrate:fresh -seed) - if seeding goes with errors


composer require guzzlehttp/guzzle - in gateway folder

composer require dusterio/lumen-passport 
php artisan migrate
php artisan passport:install

Admin Zone:
composer create-project laravel/laravel AdminZone
php artisan serve
composer require guzzlehttp/guzzle
.env - sqlite  + database/database.sqlite file
php artisan migrate
php artisan migrate:fresh - + after db structure change
php artisan make:auth
php artisan make:controller WelcomeController