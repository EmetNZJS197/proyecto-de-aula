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
