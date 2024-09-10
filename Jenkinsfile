pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Fetch the code from GitHub
                git 'https://github.com/Swap254/sample-repo.git'
            }
        }

        stage('Run Python Script') {
            steps {
                // Run your Python script
                bat 'python path/to/math_operations.py'
            }
        }

        stage('Run Tests') {
            steps {
                // Run your unit tests
                bat 'python -m unittest discover'
            }
        }
    }
}
