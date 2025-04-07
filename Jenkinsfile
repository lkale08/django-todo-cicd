pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git url: 'https://github.com/lkale08/todo-cicd.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Run Tests') {
            steps {
                sh 'npm test'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
    }
}
