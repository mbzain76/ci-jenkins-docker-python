pipeline {
    agent { docker { image 'python:3.7' } }
    stages {
        stage('Build') {
            steps {
                // Download the code
                checkout scm
            }
        }
        stage('Test') {
            steps {
                // Run the tests
                sh 'python test_calculator.py'
            }
        }
    }
}
