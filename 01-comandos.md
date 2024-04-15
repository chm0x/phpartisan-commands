# Comandos para Laravel

## Create project
```
$ composer create-project laravel/laravel project-name

# With prefer-dist
$ composer create-project laravel/laravel project-name --prefer-dist

# Create a project with a specific version of laravel
$ composer create-project laravel/laravel project-name "10.0.*"
$ composer create-project laravel/laravel project-name "5.*"
```




## Basics

Help command
```
$ php artisan help
```

List command
```
$ php artisan list
```

List Laravel Version
```
$ php artisan about
$ php artisan --version
```

## Servidor
```
# Servidor On 
$ php artisan server
```

## Routes

List Routes
```
$ php artisan route:list
```

## Controller

Create controller
```
$ php artisan make:controller NameController
```

### Resource

```
$ php artisan make:controller NameController --resource
```

## MIDDLEWARE

```
$ php artisan make:middleware NameMiddleware
```

## Database

### Create Migration
```
$ php artisan make:migration create_tablename_table
$ php artisan make:migration create_tablename_table --table=tablename

# i.e
$ php artisan make:migration create_usuarios_table
$ php artisan make:migration create_usuarios_table --table=usuarios
```

### Migrate
```
$ php artisan migrate 
```

### Refresh

when you are adding a new column on a existing table, you must use this command to migrate:
```
$ php artisan migrate:refresh
```

### SEEDERS

El proposito es rellenar la(s) tabla(s) para hacer experimentos. 

```
$ php artisan make:seed name_seed

# i.e
$ php artisan make:seed frutas_seed
```

#### Run seeder
```
$ php artisan db:seed --class=frutas_seed
```

### Rollback
```
$ php artisan migrate:rollback
```

