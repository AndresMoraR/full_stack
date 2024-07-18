# Full Stack

Para ejecutar el aplicativo se debe instalar Mysql 5.6 con un servidor apache con la versión PHP 7.2:

 - Crear una base de datos en blanco que se llame: prueba_fullstack_s1
 - Crear una segunda base de datos en blaco que se llame: prueba_fullstack_s2
 - Clonar este repositorio en la ubicación del servidor apache en la carpeta prueba_fullstack_2.
 - Abrir una primera consola y dirigirse a la ruta: ..\prueba_fullstack_2\backend
 - Ejecutar el siguiente comando: composer require codeigniter4/framework
 - Ejecutar el siguiente comando: composer update
 - Ejecutar la migración de las tablas ejecutando el siguiente comando: php spark migrate
 - Eejecutar los seeders con los siguientes comandos:
    php spark db:seed ExcepcionSeeder
    php spark db:seed FuncionarioSeeder
 - Ejecutar el siguiente comando para iniciar la aplicación donde se encuentran los servicios: php spark serve (No cerrar)
 - Abrir una segunda consola y dirigirse a la ruta: ..\prueba_fullstack_2\frontend 
 - Ejecutar el comando: npm install
 - Ejecutar el siguiente comando para iniciar la aplicación vue.js: npm run serve (No cerrar)
 - Al terminar debe dirigirse al explroador web e ingrear al siguiente enlace: http://localhost:8081/ donde podra hacer uso de la aplicación.

Los servicios se pueden testear en postman por medio de las siguientes url:
 - Generación de tokens: http://localhost:8080/auth/generate
 - Consulta de todos los datos ingresados en el formulario: http://localhost:8080/funcionario
 - Creación de nuevo registro de formulario: http://localhost:8080/funcionario/store
 - Consulta de todas las excepciones: http://localhost:8080/excepcion/
 - Creación de nuevo registro de expceciones: http://localhost:8080/excepcion/store
 - Consulta de las excepciones filtradas por fecha: http://localhost:8080/excepcion/filterDate
