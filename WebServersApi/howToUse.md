cd into api folder and run "php -S localhost:8000 -t public" there, 8001 for next api, etc.

create database/database.sqlite file

.env - DB_CONNECTION=sqlite, # the rest DB_

APP_KEY - generate 32 char and paste/save

composer require guzzlehttp/guzzle - in gateway folder

composer require dusterio/lumen-passport 

php artisan migrate

php artisan passport:install

php artisan passport:client
no user - empty user ID - hit enter with no input
name - MyClient
redirect - empty
--> new clent Id and secret

