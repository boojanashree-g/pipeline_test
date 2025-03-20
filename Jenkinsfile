pipeline {
    agent any  // Use any available agent

    environment {
        IMAGE_NAME = "myapp:latest"
        CONTAINER_NAME = "myapp-container"
    }

    stages {
        stage('Clone Repository') {
            steps {
                echo 'Cloning the repository...'
            }
        }

        stage('Install Dependencies') {
            steps {
                echo 'Installing dependencies...'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                echo 'Building Docker image...'
                echo 'Stopping existing container if running...'
                echo 'Running new Docker container...'
            }
        }
    }

    post {
        success {
            echo "Pipeline executed successfully!"
        }
        failure {
            echo "Pipeline failed!"
        }
    }
}
