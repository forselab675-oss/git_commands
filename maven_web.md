# MAVEN WEB COMMANDS

```bash
# Check Maven version
mvn -version

# Create Maven Web project
mvn archetype:generate -DgroupId=com.example -DartifactId=HelloWeb -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false

# Enter project directory
cd HelloWeb

# Compile the project
mvn compile

# Clean project
mvn clean

# Package the project into WAR
mvn package

# Install project
mvn install

# Run tests
mvn test

# Validate project
mvn validate

# Clean and package
mvn clean package
```

## Deploy WAR file to Tomcat

```bash
# Copy WAR file to Tomcat webapps directory
cp target/HelloWeb.war /path/to/tomcat/webapps/

# Start Tomcat
/path/to/tomcat/bin/startup.sh

# Stop Tomcat
/path/to/tomcat/bin/shutdown.sh
```

## Access web application

```text
http://localhost:8080/HelloWeb
```
