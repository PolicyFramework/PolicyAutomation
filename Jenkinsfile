pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sshagent(credentials :['ssh-ubuntu']) {
                   sh """
                   ssh -tt -o stricthostkeychecking=no admin123@192.168.49.1
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
