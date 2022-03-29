pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sshagent(credentials :['ssh-ubuntu']) {
                   sh """
                   ls ~/policies
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
