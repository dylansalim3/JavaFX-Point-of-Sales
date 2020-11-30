# JavaFX-Point-of-Sales
Point of Sales with inventory management system 

The MIT License (MIT)

Copyright (c) 2013 Thomas Park

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

# Prerequisite
- Java 1.8 (Only Java 8 have JavaFX built into the SDK, after Java 8 will need to include the JavaFX dependencies to the project)
- Maven 3
- MySQL

# Setup
1. Create a new Database called "inventory" and run the inventory.sql to create tables and insert the data
2. Change the connection credentials in the hibernate.cfg.xml. Change the port, mysql username and password
`
    <property name="hibernate.connection.url">jdbc:mysql://localhost:3300/inventory</property>
        <property name="hibernate.connection.username">root</property>
        <property name="hibernate.connection.password">password</property>
`
3. Set Java and Maven to its environmental variable
`
    //Check java version, make sure it is 1.8.*
    java -version

    //Check maven version
    mvn -version
`
4. Run the following command on the root folder of the project
`
    mvn clean
    mvn package
    cd target
    java -jar inventory-1.0.jar
`

# Login Credential
Username: admin
Password: admin