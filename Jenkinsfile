pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/varsshhhhhhha/CalculatorApp.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean compile'
                sh 'mvn clean test'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
