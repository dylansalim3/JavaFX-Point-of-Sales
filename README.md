# JavaFX-Point-of-Sales
Point of Sales with inventory management system 

# Prerequisite
- Java 1.8 (Only Java 8 have JavaFX built into the SDK, after Java 8 will need to include the JavaFX dependencies to the project)
- Maven 3
- MySQL

# Setup
1. Create a new Database called "inventory" and run the inventory.sql to create tables and insert the data
2. Change the connection credentials in the hibernate.cfg.xml. Change the port, mysql username and password
    ```
    <property name="hibernate.connection.url">jdbc:mysql://localhost:3300/inventory</property>
    <property name="hibernate.connection.username">root</property>
    <property name="hibernate.connection.password">password</property>
    ```
3. Set Java and Maven to its environmental variable
    ```
    //Check java version, make sure it is 1.8.*
    java -version

    //Check maven version
    mvn -version
    ```
4. Run the following command on the root folder of the project
    ```
    mvn clean
    mvn package
    cd target
    java -jar inventory-1.0.jar
    ```

# Login Credential
Username: admin <br>
Password: admin