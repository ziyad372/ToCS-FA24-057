pipeline {
    agent any

    tools {
        jdk "JDK17"
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
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
}