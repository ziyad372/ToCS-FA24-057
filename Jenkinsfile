pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
    
                sh 'javac Main.java'
            }
        }

        stage('Run') {
            steps {
    
                sh 'java Main'
            }
        }
    }
}