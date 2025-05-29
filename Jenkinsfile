pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Zohaibi099/sp22-bcs-028.Quiz-3.git'
            }
        }

        stage('Compile') {
            steps {
                bat 'javac src\\Main.java'
            }
        }

        stage('Run') {
            steps {
                bat 'java -cp src Main'
            }
        }
    }
}
