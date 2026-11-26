
pipeline {
    agent any

    stages {
        stage('Start') {
            steps {
                echo 'Starting Jenkins Build'
            }
        }

        stage('Execute Script') {
            steps {
                bat 'hello.bat'
            }
        }

        stage('Finish') {
            steps {
                echo 'Build Completed Successfully'
            }
        }
    }
}
