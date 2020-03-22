# YYJLocalsForLocals Laravel Development Environment

### Included in this environment

[Laravel 7](https://laravel.com/docs/7.x)

I've added the Argon Dashboard Laravel:
- [Laravel Package](https://github.com/laravel-frontend-presets/argon)
- [Argon Dashboard Laravel](https://www.creative-tim.com/product/argon-dashboard-laravel)

[MariaDB](https://mariadb.org/)
- [A free and open source version of MySQL, widely used and supported](https://en.wikipedia.org/wiki/MariaDB)

[PHP Composer](https://getcomposer.org/)

More stuff ...

### How to run this environment

1. [Install Docker](https://www.docker.com/get-started)
2. Clone this project / repo:
```
git clone git@github.com:yyjlocalsforlocals/yyjlocalsforlocals-laravel.git
```
3. Using a terminal navigate into the directory where you have cloned the project:
```
cd /location/of/your/project
```
4. Create .env files from examples 
```
cp .env.example .env
cp app/.env.example app/.env 
```
5. Create app key
```
cd /location/of/your/project
php artisan key:generate
```
6. Install the Argon Dashboard styles and presets: 
In your project directory:
```
php artisan ui vue --auth

php artisan ui argon

php artisan migrate --seed

npm install && npm run dev
``` 

7. Start the environment with `docker-compose`
```
docker-compose up --build
```

8. [Navigate to: http://localhost:3000](http://localhost:3000)