pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'npm install'  // Install dependencies
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'npm test'  // Run your tests
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to production...'
                // Replace this with actual deploy steps (e.g., upload to server, push to cloud, etc.)
                sh 'echo "Deploying app..."'
            }
        }
    }

    post {
        success {
            echo 'Build and Deploy successful!'
        }
        failure {
            echo 'Build or Deploy failed.'
        }
    }
}
