pipeline {
    agent any

    environment {
        IMAGE_NAME = "jenkins-demo-app"
        DOCKER_IMAGE_TAG = "latest"
    }

    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }

        stage('Docker Build') {
            steps {
                script {
                    sh "docker build -t ${IMAGE_NAME}:${DOCKER_IMAGE_TAG} ."
                }
            }
        }
    }
}
