pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ PES1UG21CS450-1.cpp -o PES1UG21CS450-1'
                    python hello.py
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    sh './PES1UG21CS450-1'
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
