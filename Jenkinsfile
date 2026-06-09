pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'git@github.com:m7md-a7md14/devops-project.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t devops-app:latest ./app'
            }
        }

        stage('List Images') {
            steps {
                sh 'docker images'
            }
        }
    }
}
