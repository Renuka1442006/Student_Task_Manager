pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Renuka1442006/Student_Task_Manager.git'
            }
        }

        stage('Check Node.js and npm') {
            steps {
                bat 'node --version'
                bat 'npm --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Automated Testing') {
            steps {
                bat 'npm test'
            }
        }
    }
}