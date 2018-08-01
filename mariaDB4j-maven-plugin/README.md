# mariadb4j-maven-plugin
Maven plugin that starts and stops a MariaDB instance for the integration test phase.

This is a Maven plugin wrapper around https://github.com/vorburger/MariaDB4j, a 
helpful tool for launching MariaDB from Java. 

See pom and integration test in https://github.com/vorburger/MariaDB4j/tree/mariaDB4j-maven-plugin/mariaDB4j-maven-plugin/src/it/mariadb4j-maven-plugin-test-basic  for usage example.

## How to upgrade from mike10004 to vorburger
to upgrade from mike10004 to vorbuger version please change

```xml
<plugin>
    <groupId>com.github.mike10004</groupId>
    <artifactId>mariadb4j-maven-plugin</artifactId>
    ...
</plugin>
```

to

```xml
<plugin>
    <groupId>ch.vorburger.mariaDB4j</groupId>
    <artifactId>mariaDB4j-maven-plugin</artifactId>
    ...
</plugin>
```

###Configuration name changes
To match MariaDB4j naming standards configuration:
createDatabase -> databaseName
