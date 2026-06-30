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
                script {
                    sh 'docker build -t devops-website .'
                }
            }
        }

        stage('List Images') {
            steps {
                sh 'docker images'
            }
        }

    }
}