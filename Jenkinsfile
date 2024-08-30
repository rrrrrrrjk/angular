pipeline {
    agent any

    stages {
        stage('git clone') {
            steps {
                git branch: 'main', url: 'https://github.com/rrrrrrrjk/angular.git'
            }
        }
        stage('stop container'){
            steps {
                sh 'docker compose down'
            }
        }
        stage('start container'){
            steps {
                sh 'docker compose up -d'
            }
        }
        stage('check'){
            steps {
                sh 'docker ps'
            }
        }
    }
}
