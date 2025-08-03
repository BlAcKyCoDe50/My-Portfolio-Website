pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo '🔁 Checking out code...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo '🏗️ Building the project...'
                // Example: sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                echo '🧪 Running tests...'
                // Example: sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 Deploying the application...'
                // Example: sh './deploy.sh'
            }
        }
    }

    post {
        success {
            echo '✅ Build succeeded!'
        }
        failure {
            echo '❌ Build failed!'
        }
    }
}
