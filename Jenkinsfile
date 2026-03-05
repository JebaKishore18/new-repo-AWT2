pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/JebaKishore18/new-repo-AWT2.git'
            }
        }
        stage('Build') {
            steps {
               bat '''
               cd AWT_2
               javac jen.java
               '''
            }
        }
        stage('Execute') {
            steps {
                bat '''
                cd AWT_2
                java jen
                '''
            }
        }
    }
}
