pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Checkout GIT') {
            steps{
                git branch: 'main',
                url: 'https://github.com/mohamed-dhia-ben-amar/DevOpsJenkinsTest.git'
            }
        }
        stage('Testing Maven') {
            steps {
                sh """mvn -version"""
            }
        }
    }
}
