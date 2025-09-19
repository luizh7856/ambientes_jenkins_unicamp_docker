pipeline {
    agent any

    environment {
        PATH = "/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    }

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