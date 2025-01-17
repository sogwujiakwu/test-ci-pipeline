pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/sogwujiakwu/test-ci-pipeline.git'
            }
        }
        stage('Build') {
            steps {
                sh './build.sh'
            }
        }
        stage('Test') {
            steps {
                sh './test.sh'
            }
        }
        stage('Deploy') {
            steps {
                sh './deploy.sh'
            }
        }
    }
}
