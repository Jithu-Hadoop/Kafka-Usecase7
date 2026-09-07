pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code from Git...'
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Installing dependencies...'
                sh 'node -v'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'node test.js'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application... (placeholder)'
            }
        }
    }
    post {
        success { echo 'Pipeline succeeded!' }
        failure { echo 'Pipeline failed — check logs above.' }
    }
}
