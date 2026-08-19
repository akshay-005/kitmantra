pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Code checked out from Git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building application...'
                bat 'echo Build completed'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'echo Tests passed'
            }
        }

        stage('Finish') {
            steps {
                echo 'Pipeline completed successfully!'
            }
        }
    }

    post {
        success {
            echo 'BUILD SUCCESSFUL'
        }

        failure {
            echo 'BUILD FAILED'
        }
    }
}