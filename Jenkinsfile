pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
               powershell 'mvn clean'
               
            }
        }
        stage('Artifacts') {
            steps {
                echo 'Testing..'
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
