# Docker Compose nginx + php7 skeleton

This is a skeleton for docker compose with two containers, one running **nginx** stable version, and the other one running **PHP-FPM 7.0.x**.

## Usage

Copy `docker-compose.example.yml` to `docker-compose.yml` and adjust as needed.

Put your web application code inside `www` folder and run `docker-compose up`. Or, if you have your application files stored somewhere else, adjust the path for volumes in `docker-compose.yml`

To install additional PHP extensions, edit `docker-build/phpfpm/Dockerfile`, add `RUN docker-php-ext-install -j$(nproc) name-of-extension` and rebuild the containers, either by running `docker-compose up --build` or `docker-compose build`.

## Additional information

For more information about the containers check their documentation:

- https://hub.docker.com/_/nginx/
- https://hub.docker.com/_/php/