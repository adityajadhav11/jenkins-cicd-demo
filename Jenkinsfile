pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo '🔧 Building the application...'
            }
        }

        stage('Test') {
            steps {
                echo '✅ Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                sh 'docker build -t my-python-app .'
                sh 'docker run -d -p 5000:5000 --name python-app my-python-app'
            }
        }
    }
}
