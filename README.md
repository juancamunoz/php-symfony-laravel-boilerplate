# Laravel boilerplate

This repository contains the basic configuration for a complete local environment for Laravel Projects

### Content:
- NGINX 1.19 container to handle HTTP requests
- PHP 8.0 container to host your Laravel application
- MySQL 8.0 container to store databases

### Installation:
- Run `make build` to create all containers
- Run `make start` to spin up containers
- Enter the PHP container with `make ssh-be`
- Install your Laravel app with `composer create-project laravel/laravel app-name`
- Move the content to the root folder with `mv app-name/* . && mv app-name/.env .`. This is necessary since Composer won't install the project if the folder already contains data.
- Copy the content from `app-name/.gitignore` and paste it in the root's folder `.gitignore`
- Remove `app-name` folder (not needed anymore)
- Navigate to `localhost:1000` so you can see the Symfony welcome page :)

