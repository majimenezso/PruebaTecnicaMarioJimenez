Prueba Técnica Mario Jimenez. Desarrollo de prueba tecnica Java doublevpartners

Pre-requisitos instalaciones

Java JDK 17,22,11
Eclipse IDE for Enterprise Java and Web Developers - 2024-09 API
Docker : docker desktop
Imagen Mysql 8.0
Cursor o VS code
Mysql workbench 8.0
Node js

Instalación 🔧
Descomprimir el archivo RAR PruebaTecnicadoublevpartners (carpeta api rest - api en java sprint boot , carpeta base de datos - archivo base de datos script carpeta frontendpruebatecnica - carpeta de proyecto angular 19 material)
instalar la imagen mysql 8.0 en docker
Crear el contenedor y el volumen mediante el comando en cmd docker run -p 3310:3306 --name pruebatecnica -e MYSQL_ROOT_PASSWORD=pass -d mysql:8.0 ( se deja los archivos de imagen, del contenedor y del volumen docker para su descargar en el archivo de texto)
Opcional : restaurar la imagen , el contedor y el volumen docker mediante los comandos docker ( 1. docker load -i mysql_8.0_backup.tar, 2. docker run --rm -v bf7eca816f1b6311c98e17686a806d357cd3215a565cc919d250ff3c2d0113f2:/data -v C:/Users/User:/backup busybox tar xzf /backup/mysql_data_backup.tar -C /data --strip-components=1, 3.docker import pruebatecnica_backup.tar pruebatecnica_restored, 4. docker run -d --name pruebatecnica_restored -v /ruta/donde/guardar/mysql_data:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=pass -p 3310:3306 mysql:8.0 )
conectarse a mysql workbench con la credenciales Hostname : 127.0.0.1 puerto : 3306 username : root password : pass
ejecutar el script de la carpeta base de datos/basededatosprueba.sql en mysql workbench
importar la api rest/prueba en eclipse IDE mediante la importacion de maven
ejecutar el api mediante run java application
abrir el proyecto de la carpeta frontend/frontendpruebatecnica con vs code o cursor
instalar las dependencias de angular
instalar angular cli
ejecutar el comando ng serve para ejecutar el frontend en el navegador y consumir el api OPCIONAL si es necesario instalar las dependencias instalarlas con npm install
se deja PDF de las evidencias realizadas a la prueba y el documento guia para la instalacion y funcionamiento en local de la prueba
