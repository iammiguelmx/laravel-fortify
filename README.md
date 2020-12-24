<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

# Laravel Fortify

Laravel Fortify es un proyecto sencillo el cual permite registrar usuarios, verificar correo, resetear contraseña, e iniciar sesión.

## Requisitos

* Docker
* PHP 7.x
* mysql    (Imagen de Docker)
* Editor   (Visual Studio Code, Atom ,etc).

Corra en Docker: 

docker run -p 3306:3306 -d --name mysql -e MYSQL_ROOT_PASSWORD=pass mysql/mysql-server


## Installation
Primero clone este repositorio:

```bash
$git clone https://github.com/iammiguelmx/laravel-fortify.git
```

Instalar las dependecias requeridas por Laravel.

```bash
$composer install
```

Configure .env y corra las migraciones.
```bash
# create copy of .env
$ cp .env.example .env

# create Laravel key
$ php artisan key:generate

# run migration
$ php artisan migrate
```

## Usage
```bash
$php artisan serve
```

Check: 
http://127.0.0.1:8000/


## Contribuciones
Las solicitudes de extracción son bienvenidas. Para cambios importantes, abra un problema primero para discutir qué le gustaría cambiar.

Asegúrese de actualizar las pruebas según corresponda.

## License
[MIT](https://choosealicense.com/licenses/mit/)
