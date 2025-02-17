<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Docker Laravel

### Build the Docker images:

```
docker-compose build
 ```

### Start Docker Container

```
docker-compose up -d
```

### Install PHP dependencies:

``` 
docker-compose run --rm composer install
 ```

### Install Node dependecies:

``` 
docker-compose run --rm npm install
 ```

### Build asset

``` 
docker-compose run --rm npm run build
 ```

### To run the Vite development server:

```
docker-compose run --rm --service-ports npm run dev
```

### Create a copy of the .env file:

``` 
cp src/.env.example src/.env
```

### Generate an application key:

``` 
docker-compose run --rm artisan key:generate
```

### Update your database connection details in .env file

```
DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=laravel_docker
DB_USERNAME=root
DB_PASSWORD=root
```

### setup mail

```
DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=laravel_docker
DB_USERNAME=root
DB_PASSWORD=root
```

### Run database migrations:

```
docker-compose run --rm artisan migrate
```

### docker-compose run --rm artisan migrate

```
docker-compose run --rm artisan migrate 
```
