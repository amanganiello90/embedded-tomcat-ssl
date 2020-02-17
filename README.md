# Embedded-tomcat-ssl

Questo è un quick start per usare tomcat-embedded con jks (certificato ssl).

## Build the project

```
mvnw clean install
```

## Start the embedded Tomcat server

```
mvnw tomcat7:run
```

Si avrà allora:

```
[INFO] Scanning for projects...
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building How To Run Embedded Tomcat with Maven 0.0.1-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] >>> tomcat7-maven-plugin:2.2:run (default-cli) @ how-to-run-embedded-tomcat-with-maven >>>
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ how-to-run-embedded-tomcat-with-maven ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 0 resource
[INFO]
[INFO] --- maven-compiler-plugin:2.3.2:compile (default-compile) @ how-to-run-embedded-tomcat-with-maven ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] <<< tomcat7-maven-plugin:2.2:run (default-cli) @ how-to-run-embedded-tomcat-with-maven <<<
[INFO]
[INFO] --- tomcat7-maven-plugin:2.2:run (default-cli) @ how-to-run-embedded-tomcat-with-maven ---
[INFO] Running war on http://localhost:9090/
[INFO] Creating Tomcat server configuration at C:\JavaCreed\examples\maven\How To Run Embedded Tomcat with Maven\target\tomcat
[INFO] create webapp with contextPath:
Mar 20, 2014 4:00:05 PM org.apache.coyote.AbstractProtocol init
INFO: Initializing ProtocolHandler ["http-bio-9090"]
Mar 20, 2014 4:00:05 PM org.apache.catalina.core.StandardService startInternal
INFO: Starting service Tomcat
Mar 20, 2014 4:00:05 PM org.apache.catalina.core.StandardEngine startInternal
INFO: Starting Servlet Engine: Apache Tomcat/7.0.47
Mar 20, 2014 4:00:07 PM org.apache.coyote.AbstractProtocol start
INFO: Starting ProtocolHandler ["http-bio-9090"]
```


Apri il browser.

```
http://localhost:9090/hello
```

![Embedded Tomcat](img/Embedded-Tomcat.png)

