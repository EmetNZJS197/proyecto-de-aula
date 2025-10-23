# 💳 AppBank

Aplicación bancaria simulada desarrollada con **Spring Boot**, que emula el funcionamiento básico de una app tipo **Bancolombia** o **Nequi**, permitiendo la gestión de clientes y cuentas bancarias a través de un backend en spring boot.

---

## Características principales

- Datos gestionados desde archivos JSON (`customers.json`, `accounts.json`), puesto que durante el proyecto no se implementó una conexión con una base de datos, por lo cual se da uso a extensiones de la IDE Visual Studio Code(`extension thunder Client`) para insertar los datos en dichos .JSON  y hacer uso del programa; de lo contrario este presentara un error por falta de los datos necesarios para la ejecucion del programa. 
- Arquitectura modular con separación entre controladores, servicios y modelos (comunmente conocida como `MVC modelo-vista-controlador`), lo que permite un codigo limpio, estructurado y escalable.

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

## FUTURAS MEJORAS QUE SE PUEDEN TENER EN CUENTA

- Implementacion de una base de datos con MySQL mediante la implementacion de la libreria `mysql-connector-j`
- Implementacion de un frontend con dependencias como `Thymeleaf`y asi darle diseño, funcionalidad e interactividad con lenguages como `HTML`, `CSS` y `JavaScript/TypeScript`
- Implementar un servidor para que dicha aplicacion funcione en la red y no solo como proyecto de aula sino tambien sea lanzada como una aplicacion de uso cotidiano la cual resuelva el problema de servicios de acceso financiero, como pagos, trasnferencias, consultas de saldos de manera comoda y digital

---

## TECNOLOGIAS Y DEPENDENCIAS

-- Java17+
-- Springboot 3.5.6
-- Springweb
-- Spring-boot-devtools
-- Maven
-- JSON
-- Javadoc

---

## EJECUCION DEL PROYECTO

-- Tener instalado Java 17 o superior
-- Tener Maven configurado
-- Ejecutar esto en una IDE como `Visual Studio Code`
-- Iniciar la aplicacion desde el `Main.java` y fijarse en el puerto inicializado por el servidor `TOMCAT`
-- ingresar al navegador con la direccion `localhost:(puerto dado)`
-- Ingresar los datos a los archivos .JSON con `Thunder Client`
-- DIsfrutar

---

## COMANDOS DE EJECUCION EN LINUX

-- mvn clean package
-- mvn spring-boot:run o java -jar target/appbank-0.0.1-SNAPSHOT.jar (requiere instalacion de maven y compilador de java)

## LICENCIA

- Juan Sebastian Rios Rodriguez
- Proyecto académico desarrollado en el marco del curso proyecto de aula
