pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t flask-app-image .'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "No tests to run for now"'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                    docker stop flask-app || true
                    docker rm flask-app || true
                    docker run -d --name flask-app -p 5000:5000 flask-app-image
                '''
            }
        }
    }
}
