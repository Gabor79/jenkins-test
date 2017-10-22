def shortCommit ='UNKNOWN'
pipeline {
    agent any
    stages {
        stage('Build') {
            script{
                "mvn clean install"
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