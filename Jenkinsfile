pipeline {
    agent any
    stages {
        stage('Clone repository') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Bhanuprabhas1234/PES1UG22CS642_Jenkins.git'
            }
        }
        stage('Build application') {
            steps {
                sh 'g++ -o PES1UG22CS642-1 main.cpp'  
            }
        }
        stage('Test application') {
            steps {
                sh './PES1UG22CS642-1'  
            }
        }
        stage('Deploy application') {
            steps {
                echo 'Deploying application...'  
            }
        }
    }
    post {
