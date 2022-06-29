FROM laravelsail/php80-composer
WORKDIR laravel-realworld-example-app

COPY . .



RUN apt-get update && apt-get install -y sqlite3 && composer install && cp .env.example .env

CMD ["php", "artisan", "serve", "--host=0.0.0.0", "--port=8000"]
