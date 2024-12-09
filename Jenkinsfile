pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/ziyad372/ToCS-FA24-057.git'
            }
        }

        stage('Build') {
            steps {
                sh 'javac Test.java'
            }
        }

        stage('Run') {
            steps {
                sh 'java Test'
            }
        }
    }

    post {
        always {
            cleanWs()
        }
    }
}