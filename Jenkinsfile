pipeline {
    agent any
        tools {
        maven 'Maven 3.x' // Use the correct Maven name
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/varsshhhhhhha/CalculatorApp.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean compile test -X'
                
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
