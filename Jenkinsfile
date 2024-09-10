pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Swap254/sample-repo.git'
            }
        }
        stage('Build') {
            steps {
                script {
                    // Replace 'echo' with Windows compatible commands if needed
                    echo 'Building the project...'
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    // Replace 'echo' with Windows compatible commands if needed
                    echo 'Running tests...'
                }
            }
        }
    }
}
