pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Fetch the code from GitHub
                git 'https://github.com/Swap254/sample-repo.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                // Install any required dependencies using batch commands
                bat 'pip install -r requirements.txt'
            }
        }

        stage('Run Python Script') {
            steps {
                // Execute your Python script using batch commands
                bat 'python math_operations.py'
            }
        }

        stage('Run Tests') {
            steps {
                // Execute your unit tests using batch commands
                bat 'python -m unittest discover'
            }
        }
    }
}
