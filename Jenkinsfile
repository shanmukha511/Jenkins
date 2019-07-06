pipeline {
    agent {
        
        docker {
            
            label "UnixSlave"
            image 'node:7-alpine' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
