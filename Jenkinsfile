pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Building Docker image
                    sh 'docker build -t cm-kg-projectname .'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    // Run tests or validation steps here if any
                    echo 'No tests for this project'
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    // Deployment steps here if needed
                    echo 'Deploying application'
                }
            }
        }
    }

    post {
        always {
            echo 'Cleaning up'
            sh 'docker system prune -f'
        }
    }
}
