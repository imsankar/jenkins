pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
               powershell 'mvn clean'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
