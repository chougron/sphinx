# Sphinx

Sphinx is a website to solve or create riddles. Log in and start solving riddles created by others, or create your own sequence of questions for other users to play.

Sphinx is based on <a href="https://laravel.com" target="_blank">Laravel</a>

## Requirements

* PHP 7.4+ (check [extensions requirements for Laravel](https://laravel.com/docs/8.x#server-requirements))
* Composer
* SQL Database (this project was developed using Postgres)

## Installation

Install the packages using `composer install`.

Copy `.env.example` to your own `.env` file, and configure the different values. You can use `php artisan key:generate --ansi` to generate a random __APP_KEY__

Give permissions to the folders __storage__ and __bootstrap/cache__ and all their subfolders so the web server can access and write on them.
For example :

```
chown $USER:www-data -R storage bootstrap/cache
chmod 775 -R storage bootstrap/cache
```

Install the database migration system with `php artisan migrate:install`, then launch the migrations for the database with `php artisan migrate`.

## License

Sphinx is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
