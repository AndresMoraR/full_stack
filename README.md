# Prueba Full Stack

Para ejecutar el aplicativo se debe instalar Mysql 5.6 con un servidor apache con la versión PHP 7.2:

1- Crear una base de datos en blanco que se llame: prueba_fullstack_s1
2- Crear una segunda base de datos en blaco que se llame: prueba_fullstack_s2
3- Clonar este repositorio en la ubicación del servidor apache en la carpeta prueba_fullstack_2.
4- Abrir una primera consola y dirigirse a la ruta: ..\prueba_fullstack_2\backend
composer require codeigniter4/framework
composer update
5- Sobre la ruta anterior ejecutar la migración de las tablas ejecutando el siguiente comando: php spark migrate
- Abrir una segunda consola y dirigirse a la ruta: ..\prueba_fullstack_2\frontend y ejecutar el comando: npm run serve
- Dirigirse a un explroador web y dirigirse al siguiente enlace: 
