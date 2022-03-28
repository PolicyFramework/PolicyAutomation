pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Establishing Remote SSH Connection...'
                sh 'ssh admin123@192.168.49.1'
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
