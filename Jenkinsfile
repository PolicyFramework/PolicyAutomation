pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Establishing Remote SSH Connection...'
                sh 'ssh -o StrictHostKeyChecking=no admin123@192.168.49.1 uptime'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
