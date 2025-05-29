pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the main branch from your GitHub repo
                git branch: 'main', url: 'https://github.com/Zohaibi099/sp22-bcs-028.Quiz-3.git'
            }
        }

        stage('Compile Java') {
            steps {
                // Compile the Java file Hello.java inside the Quiz03 folder
                bat 'javac Hello.java'
            }
        }

        stage('Run Java') {
            steps {
                // Run the Hello class from Quiz03 folder (use -cp to specify classpath)
                bat 'java Hello'
            }
        }
    }
}
