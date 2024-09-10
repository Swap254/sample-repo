pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Fetch the code from your GitHub repository
                git 'https://github.com/Swap254/sample-repo.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                // Install any required dependencies (if you have a requirements file)
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run Python Script') {
            steps {
                // Execute your Python script
                sh 'python math_operations.py'
            }
        }

        stage('Run Tests') {
            steps {
                // Execute your unit tests
                sh 'python -m unittest discover'
            }
        }
    }
}
