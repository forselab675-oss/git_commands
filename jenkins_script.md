# JENKINS SCRIPT COMMANDS

## 1. Create a Shell Script

nano hello.sh

# Creates or opens a shell script

## 2. Write the Script

#!/bin/bash
echo "Hello from Jenkins"

# Prints a message

## 3. Give Execute Permission

chmod +x hello.sh

# Makes the script executable

## 4. Run the Script

./hello.sh

# Executes the shell script

## 5. Start Jenkins

sudo systemctl start jenkins

# Starts Jenkins service

sudo systemctl status jenkins

# Checks Jenkins status

## 6. Jenkins Pipeline (Jenkinsfile)

pipeline {
    agent any

    stages {
        stage('Execute Script') {
            steps {
                sh 'chmod +x hello.sh'
                sh './hello.sh'
            }
        }
    }
}

# Executes the shell script through Jenkins pipeline

## 7. Run Pipeline from Jenkins

# Open http://localhost:8080
# Select New Item
# Enter project name
# Select Pipeline
# Click OK
# Select Pipeline script
# Paste the Jenkinsfile
# Click Save
# Click Build Now
# Click Console Output to view results
