pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sshagent(['ssh-ubuntu']) {
                   sh """
                   ssh -o StrictHostKeyChecking=no admin123@192.168.49.1
                   """
               }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
