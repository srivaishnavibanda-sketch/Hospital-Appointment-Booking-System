
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Downloading Hospital Appointment Booking System from GitHub'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building Hospital Appointment Booking System'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing Hospital Appointment Booking System'
                bat 'dir'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Hospital Appointment Booking System Deployment Successful'
            }
        }
    }

    post {
        success {
            echo 'Pipeline Executed Successfully'
        }
        failure {
            echo 'Pipeline Failed'
        }
    }
}
