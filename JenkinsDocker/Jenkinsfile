pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    // Build the Docker image
                    sh 'docker build -t ola-unicamp .'
                }
            }
        }
        stage('Run') {
            steps {
                script {
                    // Run the Docker container
                    sh 'docker run ola-unicamp'
                }
            }
        }
    }
}