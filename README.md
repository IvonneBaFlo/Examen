.:.Examen Práctico PHP .:.

Para realizar el desarrollo del examén, se ocupo dos sistemas. 
1. El primero y fundamental XAMPP es un software libre, que permite gestionar bases de datos MySQL y servidor APACHE para la interpretacion de codigo PHP.

Se ocupó XAMPP para Windows version 8.0.9 de la siguiente liga
https://www.apachefriends.org/es/index.html

Al terminar la descarga del archivo .exe, se ejecuta el sistema sin ningun problema instalando el paquete completo.

*Se abre XAMPP control de panel, interfaz que permite configurar los servicios con los puertos necesarios.
	- En mi caso yo tuve tema para instalar el sistema por temas de usos de puertos con los demas sistemas ya instalados.
	- Se configuro en la opcion de Config, Apache(httpd.confg), manualmente se configuro el puerto de Apache, el sistema se instalo con el puerto 80, para mi caso se cambio al puerto 8080, se actualizo el archivo y se guardo los cambios.
	Tambien se configuro  Apache(httpd-ssl.confg), manualmente se configuro el puerto de Apache, el sistema se instalo con el puerto 443, para mi caso se utilizo el 4430, se actualizo el archivo y se guardo los cambios. 
Para iniciar servicio desde la interfaz de Control de Panel, se oprime el boton Start. Y validar desde el navegador colocamos la siguiente liga con el puerto que se indico para apache 8080.
http://localhost:8080/dashboard/ Es la pagina principal de XAMPP.

Para Mysql, de la interfaz de control de panel solo se valida la configuracion de Mysql, dentro de Config(my.ini), se valida el puerto 3306. Se guardon los cambios, se inicia el servicio oprimiendo el boton de Start de MySql y validar desde el navegador colocamos la siguiente liga.

http://localhost:8080/phpmyadmin Es la pagina de phpMyAdmin la interfaz grafica para generar base de datos Mysql.

O en mi caso se genero los scripts de base de datos en SQL server,  Microsoft SQL Server 2012
El script contiene la creacion de las tablas. 
Al momento de ingresar de manera local a la gestion de base de datos.
Se crea la base de datos Examen. 
Se abre una solucion, con los siguientes comandos para la creacion de bd

USE CREATE DATABASE EXAMEN
GO
Al momento de indicar que fue generada la base de datos se genera el script para la base de datos.

Se descarga la informacion de la liga GITHUB
https://github.com/IvonneBaFlo/Examen.git
Contiene dos archivos. 
Examen.zip 
y el archivo de README.md

Se descomprime el archivo .ZIP, contiene una carpeta Examen, en ella existen dos carpetas 
* SQL y PHP
- En SQL, se encuentra el script se puede abrir desde SQL server, Archivo, Proyecto o solucion, se busca el documento antes mencionado.
- Se encuentran los scripts de las tablas que indica para el examen, con llaves primarias y relacion de tablas. 
Se ejecuta los scripts sin ningun problema. 

Para PHP, se ocupo SUBLIME TEXT para escribir y editar codigo fuente. 
Se desarrollo los siguientes archivos
Se encuentra codigo de PHP. 
Cuatro archivos 
* database que se encarga de tener la conexion de base de datos con php
* index para cargar la pagina de Inicio login
* Signup pagina de inicio de sesion
* logout pagina para cerrar sesion
Dentro del archivo se encuentra dos carpetas 
assets\css un archivo llamado style hojas de estilo para el diseño de la pagina principal.
La siguiente carpeta es dentro de PHP es partials 
donde contiene un archivo llamado header codigo fuente donde indica el nombre de la persona que lo desarrollo.

Para ejecutar el codigo antes mencionado. 
Nos dirigimos a la raiz del disco local C, donde se instalo el sistema de XAMPP y buscamos la carpeta htdocs para guardar la carpeta PHP 
C:\xampp\htdocs

Se valida en la siguiente liga
http://localhost:8080/PHP/
Se estaba generando la interfaz de login e inicio de sesion. 









