pipeline {
    agent any

    stages {
        stage('Build') {
            agent { docker { image 'python:3.6' } }
            steps {
                sh 'python --version'
                sh 'echo "omg did that really work"'
            }
        }
        stage('Test') {
            agent { dockerfile true }
            steps {
                sh 'python manage.py test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}

