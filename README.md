# Welcome to 'Taxi Service'

This is Web application simulates a work of simple taxi service. Supports authentication, registration, interaction with the database (CRUD operations).

The project is implemented in Java with SOLID principles & Dependency Injection, has a 3-tier architecture.

### Functional
- register, login and logout drivers
- display all drivers, with the possibility to delete
- display all cars, with the possibility to delete
- display cars by the driver, who is authenticated
- display all manufacturers
- create a new car
- create a new manufacturer
- add a driver to a car

### 3-layer architecture
1. DAO - Data access layer
2. Service - Application layer
3. Controllers - Presentation layer

### Technologies
- Java 11
- Tomcat - version 9.0.50
- MySQL
- JDBC
- Servlet
- JSTL
- JSP
- HTML, CSS

### How to start the program :
To correctly use this service you have to install MySQL and Apache Tomcat version 9.
- Configure Apache Tomcat for your IDE.
- Use [init.db.sql](src/main/resources/init_db.sql) for creating a schema and tables.
- Configure [ConnectionUtil](src/main/java/taxi/util/ConnectionUtil.java) with your *URL*, *USERNAME*, *PASSWORD*, *JDBC_DRIVER*.
- In the [log4j.xml](src/main/resources/log4j.xml) at line ```<File name="LogToFile" fileName="/logs/app.log">``` you need to change ```logs\app.log``` with absolute path to ```.log file```
- Configure the Tomcat library path in the startup settings.
- Start the project.

