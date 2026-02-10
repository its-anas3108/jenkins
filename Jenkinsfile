pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t python-app .'
            }
        }

        stage('Run Tests Inside Docker') {
            steps {
                sh 'docker run python-app'
            }
        }
        stage('Run Application') {
            steps {
                sh 'echo Application running'
            }
        }
    }
}
