# MAVEN JAVA COMMANDS

```bash
# Check Maven version
mvn -version

# Create Maven Java project
mvn archetype:generate -DgroupId=com.example -DartifactId=HelloMaven -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false

# Enter project directory
cd HelloMaven

# Compile the project
mvn compile

# Run tests
mvn test

# Package the project
mvn package

# Clean generated files
mvn clean

# Install project into local Maven repository
mvn install

# Run Java application
mvn exec:java -Dexec.mainClass="com.example.App"

# Validate project
mvn validate

# Display Maven version
mvn -version
```

