# Multitenancy module provide appropriate datasource connection dependeing on the first path variable (locnNbr)

# To enable multitenancy in your project, add following dependency

        <dependency>
            <groupId>io.github.spansari</groupId>
            <artifactId>multi-tenancy-spring-boot-starter</artifactId>
            <version>1.0.0-SNAPSHOT</version>
        </dependency>

# and set this property in application.properties to true

> multitenancy.enabled=true

#Create "tenants" folder at the root of the project, and add file for each locnNbr in following format:
 ###<fileName: 1234.properties>
>name=1234

>datasource.url=jdbc:mysql://127.0.0.1:3306/db1

>datasource.username=userId

>datasource.password=pwd

---
