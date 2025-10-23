pipeline {
    agent any
 
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/shriyadr68/DevOpsDemo.git'
            }
        }
 
        stage('Build') {
            steps {
                echo 'Compiling Java code...'
                sh 'javac Hello.java'
            }
        }
 
        stage('Run') {
            steps {
                echo 'Running Java code...'
                sh 'java Hello'
            }
        }
    }
}
