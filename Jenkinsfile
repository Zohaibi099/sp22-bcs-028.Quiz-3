pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'python', url: 'https://github.com/Zohaibi099/sp22-bcs-028.Quiz-3.git'
            }
        }

        stage('Setup Python') {
            steps {
                bat 'python --version'
            }
        }

        stage('Run Script') {
            steps {
                bat 'python hello.py'
            }
        }
    }
}
