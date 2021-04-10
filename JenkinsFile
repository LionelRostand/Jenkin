pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.73   uptime'
            }

        }
        stage('Test') {
            steps {
                sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.73  apt update'
                 sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.73 ls -lrt'
            }

        }


    }
}
