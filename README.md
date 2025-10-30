AppBank

Aplicación bancaria simulada desarrollada con Spring Boot, que emula el funcionamiento básico de una app tipo Bancolombia o Nequi, permitiendo la gestión de clientes y cuentas bancarias a través de un backend en Spring Boot.

---

## Características principales

- Los datos se gestionan desde archivos JSON (`customers.json`, `accounts.json`), ya que durante el desarrollo del proyecto no se implementó una conexión con una base de datos.
  Para insertar y manipular los datos se utiliza la extensión Thunder Client en la IDE Visual Studio Code, que permite realizar peticiones HTTP y modificar los archivos JSON.
  En caso de no cargar los datos correctamente, el programa generará un error por la falta de información necesaria para su ejecución.

- El proyecto sigue una arquitectura modular con separación entre controladores, servicios y modelos, comúnmente conocida como MVC (Modelo–Vista–Controlador).
  Esto permite mantener un código limpio, estructurado y escalable.

---

## Ejemplo de la estructura del proyecto

...
├── data
│   ├── accounts.json
│   └── customers.json
├── docs
│   ├── allclasses-index.html
│   ├── allpackages-index.html
│   ├── com
│   ├── copy.svg
│   ├── element-list
│   ├── help-doc.html
│   ├── index-all.html
│   ├── index.html
│   ├── legal
│   ├── link.svg
│   ├── member-search-index.js
│   ├── module-search-index.js
│   ├── overview-tree.html
│   ├── package-search-index.js
│   ├── resources
│   ├── script-dir
│   ├── script.js
│   ├── search.html
│   ├── search.js
│   ├── search-page.js
│   ├── stylesheet.css
│   ├── tag-search-index.js
│   └── type-search-index.js
├── LICENSE
├── mvnw
├── mvnw.cmd
├── pom.xml
├── README.md
├── src
│   ├── main
│   └── test
└── target
    ├── appbank-0.0.1-SNAPSHOT.jar
    ├── appbank-0.0.1-SNAPSHOT.jar.original
    ├── classes
    ├── maven-archiver
    ├── maven-status
    ├── surefire-reports
    └── test-classes
...

---

## Futuras mejoras que se pueden tener en cuenta

- Implementación de una base de datos relacional (por ejemplo, MySQL) mediante la librería mysql-connector-j.
- Creación de un frontend utilizando dependencias como Thymeleaf, con diseño e interactividad a través de HTML, CSS y JavaScript/TypeScript.
- Implementación de un servidor que permita ejecutar la aplicación en red, con el objetivo de convertirla en una herramienta funcional de uso cotidiano que facilite operaciones financieras como pagos, transferencias y consultas de saldo de forma cómoda y digital.

---

## Tecnologías y dependencias

- Java 17+
- Spring Boot 3.5.6
- Spring Web
- Spring Boot DevTools
- Maven
- JSON
- Javadoc

---

## Ejecución del proyecto

1. Tener instalado Java 17 o una versión superior.
2. Tener Maven configurado en el sistema.
3. Abrir el proyecto en una IDE como Visual Studio Code.
4. Iniciar la aplicación desde la clase Main.java y verificar el puerto asignado por el servidor Tomcat.
5. Acceder a la aplicación desde el navegador en la dirección localhost:(puerto asignado).
6. Insertar los datos en los archivos .json utilizando Thunder Client.
7. Ejecutar y utilizar la aplicación.

---

## Demostracion de Ejecucion (Pruebas Postman)

lo primero que debera hacer es abrir el proyecto y dirigirse al main, para posteriormente ejecutarlo, siendo el resultado algo como esto
<img width="1848" height="1042" alt="image" src="https://github.com/user-attachments/assets/afff5689-fc13-4af1-b5de-e63568762bd9" />

despues debera asegurarse de tener instalada la extension Thunder Client
<img width="1000" height="592" alt="image" src="https://github.com/user-attachments/assets/ec0b01f7-6326-43fc-a9af-391b3bfacd0e" />

una vez hecho esto debera irse a la pestaña de esta extension y pulsar **new request**
<img width="297" height="117" alt="image" src="https://github.com/user-attachments/assets/9412bc8d-495e-475c-9a69-69b276ecc845" />

lo primero que haremos sera crear un nuevo cliente para nuestra aplicacion ingresando la url mostrada en la foto de tipo post y se ingresaran los datos como se muestra en el body del JSON y el resultado se mostrara en la ventana derecha
<img width="1489" height="566" alt="image" src="https://github.com/user-attachments/assets/9c358d43-e647-44a3-966c-e4d50b08291a" />

a continuacion pondremos la misma url pero esta vez con el id del cliente seguido de "/accounts" y asi tendriamos nuestra cuenta creada
<img width="1489" height="566" alt="image" src="https://github.com/user-attachments/assets/6e34954c-8043-47c1-b7e0-c8218b1f3ec2" />

si usted desea buscar un cliente debera hacerlo por su id como se muestra a continuacion
<img width="1489" height="566" alt="image" src="https://github.com/user-attachments/assets/56126ab8-bee8-489b-9b90-d3d6dadbdc77" />

o si usted desea ver todos los clientes podra hacerlo de esta manera
<img width="1489" height="566" alt="image" src="https://github.com/user-attachments/assets/0ca6eda8-72db-4e53-96b6-19bb8cb0d3ae" />

para consultar las transacciones puede hacerlo de la siguiente forma
<img width="1489" height="566" alt="image" src="https://github.com/user-attachments/assets/5af11a9b-789d-4f8a-b5d2-3b83bf2a519e" />


---


## Swagger
tambien puede acceder a http://localhost:8080/swagger-ui/index.html para testear el programa en lugar de usar thunderclient y ademas observar la documentacion
aqui tiene algunos ejemplos
<img width="1448" height="580" alt="image" src="https://github.com/user-attachments/assets/de9906ae-bff3-4830-a6d0-9a953a26cd27" />
<img width="1458" height="804" alt="image" src="https://github.com/user-attachments/assets/3ab04d8c-4087-450a-99ff-27371a66df22" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ac482773-500b-4fac-8d91-be393c9b4d4d" />



---


## Comandos de ejecución en Linux

mvn clean package

mvn spring-boot:run

O bien:

java -jar target/appbank-0.0.1-SNAPSHOT.jar

(Requiere la instalación de Maven y un compilador de Java configurado correctamente.)

---

## Licencia

Proyecto académico desarrollado por Juan Sebastián Ríos Rodríguez 
en el marco del curso Proyecto de Aula.

Se hizo uso de la IA para la redacción de este documento, mas no para la realización del mismo.
