pipeline {
    agent any

    stages {
        stage('Build') {
            agent { docker { image 'python:3.6' } }
            steps {
                sh 'python --version'
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

