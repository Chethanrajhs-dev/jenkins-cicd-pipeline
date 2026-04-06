pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/yourusername/jenkins-cicd-pipeline.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t myapp .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 80:80 myapp'
            }
        }
    }
}
