pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.19    mkdir /applis'
                 sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.19   export Home_applis=/applis'
                 sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.19  chown youtechadmin:youtechadmin /applis'
            }

        }
        stage('DELTE') {
            steps {
                sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.19    rmdir /applis'
               
            }

        }
       
    }
    
}
