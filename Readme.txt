Prueba Ingreso – Fullstack
Wilmar Enrique Cardona Rodriguez
CC 100257997
Estudiante Ingeniería Informática U-Caldas



A continuación, se dará a conocer información relacionada a la solución del problema expuesto.

Tecnologías utilizadas para el BACKEND:
* IDE utilizada : eclipse 2023-09 (4.29)?
* Framework utilizada : Springboot (Spring Tools 4(aka Spring Tool 4) 4.21.1 RELEASE)
* Dependencias de Springboot ( MySQL Driver, Spring Boot DevTools, Spring Data JPA, Spring web)
Tecnologías utilizadas para el FRONTEND:
* Visual Studio Code 1.87
* Angular Language Service v17.2.2
* Angular Snippets (Version 16)
* NODE JS v21.6.2

Base de datos utilizada:
* MySQL 8.0.36
* MySQL Workbench 8.0.36

Otras tecnologías
* Postman





Anotaciones:
* Dentro de la prueba se requería el consumo de REST API, dado que esto no se encontraban en funcionamiento, creé la API de forma local para presentar la solución
* Para la ejecución de la solución se utilizan rutas únicas, en donde el usuario podrá ingresar el origen y destino, y el programa calculara la ruta para llegar al destino desde el origen, a continuación se mostrara un esquema de la ruta

Origen  - destino
col        -   arg
arg       -   bol
bol        -   par
par       -   ven
ven        -   ecu

* para el ingreso de los datos como de transport y flights se utilizó Postman para ingresar los datos como parametros
Funcionamiento de la solución:
Importante: el desarrollo de la solución fue realizado de forma local;
En el paquete adjunto encontrara la carpeta NEWSHORE_AIR,  esta carpeta contiene toda la documentación relacionada al BACKEND y dentro de la misma encontrara la carpeta relacionada al FRONTEND llamada de la siguiente manera NEWSHORE_AIR-frontend.
en el repositorio encontrara el archivo () que contiene la base de datos usada en MySQL Workbench;

1. para el funcionamiento de la solución debe importar le archivo () en MySQL Workbench.
2. La carpeta NEWSHORE_AIR que contiene la solución debe ser importada la IDE utilizado, en este caso Eclipse
3. Una vez importada la solución al IDE, puede revisar los paquetes que contiene la solución.
4. En src/main/resources encontrara el archivo de “application.properties” en donde podrá ver la conexión entre el motor de base de datos y el proyecto.
5. Dentro del proyecto encontrara 3 paquetes en la carpeta src/main/java, el primer paquete que encontrara es “com.example.NEWSHORE_AIR.Controlador” que contiene los controladores de las entidades del proyecto; dentro de cada controlador podrá encontrar la conexión hacia el Frontend
6. “@CrossOrigin(origins ="http://localhost:4200/")” 
7. El siguiente paquete es el de “ com.example.NEWSHORE_AIR.Modelo” que contiene las entidades creadas para el proyecto 
8. Por ultimo el paquete “com.example.NEWSHORE_AIR.Repositorio” que contiene archivos de tipo interface para acceder al repositorio JpaRepository

9. Para el FRONTEND abra la carpeta NEWSHORE_AIR-frontend en Visual Estudio Code, una vez abierto podrá ver que dentro de “app” se encontraran lo componentes para visualizar el Front end

10. Componente Entitys contiene las entidades creadas
11. Componente Navegador contiene el acceso a las paginas a visualizar como reservar y rutas
12. Componente Reservar contiene un formulario que solicita 2 parámetros para hacer la búsqueda de la ruta de vuelo, dentro de la misma se presentan 2 tablas, la primera ubicada a la izquierda refleja la ruta a tomar para llegar al destino, la segunda tabla ubicada bajo el formulario mostrara la información de origen, destino y el valor de la moneda seleccionada
13. Los campos del formulario reciben como máximo 3 caracteres, si estos son menores a los 3 caracteres, contienen la misma información, si se ingresan orígenes o destinos que no existan en la solución, aparecerá una alerta que corresponderá a cada situación expuesta
14. Componente rutas, contiene toda la información relacionada a los vuelos, origen destino y el precio de cada uno.
15. Componente servicio, contiene los servicios que consume la API.

16. Para ejecutar la solución, habrá que tener abierta la aplicación de MySQL Workbench, iniciar el proyecto desde el IDE, y en visual Estudio Code debe abrir un terminal de CMD y ejecutar el comando “ng serve -o”

17. Una vez ejecutado aparecerá la pagina de “reserva” en donde se visualizara lo anteriormente expuesto en “Componente Reservar” y ejecutar el programa




