# JENKINS WEB APPLICATION COMMANDS

## 1. Create Maven Web Application

mvn archetype:generate -DgroupId=com.example -DartifactId=webapp -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false

# Creates a Maven web application

cd webapp

# Enters the project folder

## 2. Build Web Application

mvn clean

# Deletes previous build files

mvn compile

# Compiles the source code

mvn test

# Runs tests

mvn package

# Creates the WAR file inside target folder

## 3. Run Jenkins

sudo systemctl start jenkins

# Starts Jenkins

sudo systemctl status jenkins

# Checks Jenkins status

## 4. Jenkins Pipeline (Jenkinsfile)

pipeline {
    agent any

    tools {
        maven 'Maven'
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}

# Defines automated build, test and packaging stages

## 5. Check WAR File

ls target/

# Displays generated WAR file
