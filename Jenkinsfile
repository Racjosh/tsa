pipeline {
    agent any
    stages {
        stage('Pull Code') {
            steps {
                git 'https://github.com/Racjosh/tsa.git'
            }
        }
        stage('Build') {
            steps {
                sh 'docker-compose down || true'
                sh 'docker-compose up -d --build'
            }
        }
    }
}
