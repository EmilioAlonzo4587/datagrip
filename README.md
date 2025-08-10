\# Guía rápida: Docker, PostgreSQL y DataGrip



**## 1... Comando para ejecutar Docker con PostgreSQL**



Para iniciar un contenedor Docker con PostgreSQL, usa el siguiente comando:



```bash

docker run --name nombre-contenedor -e POSTGRES\_PASSWORD=tu\_contraseña -p 5432:5432 -d postgres



//Reemplaza nombre-contenedor por el nombre que quieras darle al contenedor.//



//Reemplaza tu\_contraseña por la contraseña que desees para el usuario postgres.//





**2... Pasos para configurar DataGrip**



Abre DataGrip.



Ve a File > Data Sources and Drivers.



Haz clic en el símbolo + y selecciona PostgreSQL.



En la pestaña General, configura lo siguiente:



Host: localhost (si usas Docker en tu máquina local)



Port: 5432 (o el puerto que hayas elegido, en mi caso use el puerto 5433)



User: postgres



Password: la que pusiste en el comando Docker (tu\_contraseña)



Haz clic en Test Connection para verificar que está todo correcto.



Si la conexión es exitosa, haz clic en OK para guardar.



**3... Creación de la base de datos PostgreSQL desde DataGrip**



Conéctate a tu servidor PostgreSQL desde DataGrip usando la configuración anterior.



En el panel lateral, haz clic derecho sobre Databases.



Selecciona New > Database.



Escribe el nombre que quieres para tu base de datos.



Presiona Enter o haz clic en OK.



¡Listo! Ya tienes una base de datos creada y lista para usar.

