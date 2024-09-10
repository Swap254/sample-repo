pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Swap254/sample-repo.git'
            }
        }
        stage('Run Python Script') {
            steps {
                bat 'python math_operations.py'
            }
        }
    }
}
