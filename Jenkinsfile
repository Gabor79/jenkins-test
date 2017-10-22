def shortCommit ='UNKNOWN'
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat "mvn clean install"
                script{
                    shortCommit = bat(returnStdout: true, script: "git log -n 1 --pretty=format:'%h'").trim()
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