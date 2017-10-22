def shortCommit ='UNKNOWN'
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat "mvn clean install"
                script{
                    shortCommit = bat "git log -n 1 --pretty=format:'%h'"
                    echo shortCommit
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