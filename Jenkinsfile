pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.11   mkdir /applis'
                 sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.11   export Home_applis=/applis'
                 sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.11  chown youtechadmin:youtechadmin /applis'
            }

        }
        stage('DELTE') {
            steps {
                sh 'ssh -oStrictHostKeyChecking=no root@192.168.1.11   rmdir /applis'
               
            }

        }
       
    }
    
}
