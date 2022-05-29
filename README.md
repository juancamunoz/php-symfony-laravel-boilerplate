# Laravel boilerplate PHP 8 FPM, MySQL 8.0 and Ngnix with Docker & Docker Compose

This repository contains the basic configuration for a complete local environment for Laravel Projects with docker

### Content:
- NGINX 1.19 container to handle HTTP requests
- PHP 8.1 container to host your Laravel application
- MySQL 8.0 container to store databases

### Installation:
- Run `make build` to create all containers
- Run `make up` to spin up containers
- Enter the PHP container with `make ssh-be`
- Install your Laravel app with `composer create-project laravel/laravel app-name`
- Move the content to the root folder with `mv app-name/* .`. This is necessary since Composer won't install the project if the folder already contains data.
- Copy the content from `app-name/.gitignore` and paste it in the root's folder `.gitignore` and `.env, .env.example`
- Remove `app-name` folder (not needed anymore)
- Navigate to `localhost:1000` so you can see the Laravel welcome page :)

