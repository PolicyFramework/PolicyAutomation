pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sshagent(credentials :['ssh-ubuntu']) {
                   sh """
                   ssh -tt -o StrictHostKeyChecking=no admin123@192.168.49.1
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
