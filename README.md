# Install

```sh
copy .env.example .env          # set setings for database in .env
composer install
php artisan key:generate
php artisan migrate:fresh --seed
yarn install
yarn dev
```

# Development

## Linux

```sh
yarn start
php artisan serve   # open site http://localhost:8000
```

## Windows

Install <a href="https://ospanel.io/">OpenServer</a>.<br>
Install laravel.<br>
Open site from OpenServer.

```
yarn start     # for start frontend
```

# Deploy

<h5>FOR FIRST DEPLOY</h5>

```
php artisan deploy {stage} -o git_tty=true
```

```sh
php artisan deploy
```

Смотри файл config/deploy.php ! секцию hosts. Если указан stage, то
``` 
php artisan deploy {stage}
```


# Generate helpers

```
- php artisan ide-helper:meta 
- php artisan ide-helper:generate 
- php artisan sleepingowl:ide:generate
- php artisan ide-helper:models
```


