pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat "mvn clean build"
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