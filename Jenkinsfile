/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'python:3.13.5-alpine3.22' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
        stage('stage2') {
            steps {
                sh 'ping -c 4 8.8.8.8'
            }
        }
    }
}


