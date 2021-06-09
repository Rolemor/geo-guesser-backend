# geo-junkies-laravel
GEO-JUNKIES 2.0

### Summary
This that backend of a <b>GeoGuesser</b> like game.<br>
After the registration the user can choose from variety of maps to play on like <b>USA,Asia<b> or Hungary.<br>
In the game you get 5 cities whose location must be guessed on the map and closer you mark more points you will earn.

## Setup for the backend

### Use Composer to download specific dependencies
    php composer install
    
### Run migration command to create the database
You should use this command to run the migration files in the correct order.

    php artisan migrate:all:ordered
    
After the migration command don't forget to fill the .env file with the necessary data like:

    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=geo_junkies_backend
    DB_USERNAME=root
    DB_PASSWORD=password

### Seed the tables:
    php artisan db:seed
