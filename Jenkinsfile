pipeline {
    agent any

    stages {

        stage('Checkout Source') {
            steps {
                echo 'Cloning repository from github...'
                checkout scm
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'Installing node package modules...'
                bat 'npm install'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
                bat 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                echo 'Running local test script...'
                bat 'npm test'
            }
        }
    }
}
