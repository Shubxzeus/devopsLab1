pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building DevOps Lab 1...'
                bat 'dir'
                echo 'Build Completed'
            }
        }

        stage('Test') {
            steps {
                echo 'Running Tests...'
                bat 'echo Checking index.html exists'
                bat 'dir index.html'
                echo 'All Tests Passed'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying Application...'
                bat 'echo Deploying to Local Server'
                echo 'Deployment Successful'
            }
        }
    }

    post {
        success {
            echo 'Pipeline Finished: SUCCESS'
        }
        failure {
            echo 'Pipeline Finished: FAILURE'
        }
    }
}