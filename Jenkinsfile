pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script{
                    "mvn clean install"
                }
                
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