# Prueba Full Stack

Para ejecutar el aplicativo se debe instalar Mysql 5.6 con un servidor apache con la versión PHP 7.2:

1 - Crear una base de datos en blanco que se llame: prueba_fullstack_s1
2 - Crear una segunda base de datos en blaco que se llame: prueba_fullstack_s2
3 - Clonar este repositorio en la ubicación del servidor apache en la carpeta prueba_fullstack_2.
4 - Abrir una primera consola y dirigirse a la ruta: ..\prueba_fullstack_2\backend
5 - Ejecutar el siguiente comando: composer require codeigniter4/framework
6 - Ejecutar el siguiente comando: composer update
7 - Ejecutar la migración de las tablas ejecutando el siguiente comando: php spark migrate
8 - Eejecutar los seeders con los siguientes comandos:
    php spark db:seed ExcepcionSeeder
    php spark db:seed FuncionarioSeeder
9 - Ejecutar el siguiente comando para iniciar la aplicación: php spark serve (No cerrar)
10 - Abrir una segunda consola y dirigirse a la ruta: ..\prueba_fullstack_2\frontend y ejecutar el comando: npm run serve (No cerrar)
11 - Al terminar debe dirigirse a un explroador web e ingrear al siguiente enlace: 
