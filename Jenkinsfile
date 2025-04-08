pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git credentialsId: 'github-creds', url: 'https://github.com/adityajadhav11/jenkins-cicd-demo.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application using Docker...'
            }
        }
    }
}
