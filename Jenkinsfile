pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                git branch: 'main', url: 'https://github.com/rrrrrrrjk/angular.git'
            }
        }
        stage('check'){
            steps {
                sh 'docker compose up -d'
            }
        }
    }
}
