pipeline {
    agent any

    stages {
        stage('Build') {
            agent { docker { image 'python:3.6' } }
            steps {
                sh 'python --version'
                sh 'omg did that really work'
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

