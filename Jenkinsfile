pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/nausicaaandteto/jenkins-ci-test.git'
            }
        }
        stage('Build') {
            steps {
                sh 'echo "Building the app..."'
            }
        }
        stage('Test') {
            steps {
                sh 'python3 hello.py'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploy step (simulate deployment)"'
            }
        }
    }
}

