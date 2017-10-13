pipeline {
    agent {
        dockerfile {
            filename 'Dockerfile'
        }
    }
    stages {
        stage('build') {
            steps {
                withEnv(['GOPATH=' + pwd()]){
                    sh 'df -h'
                    sh 'uname -a'
                    sh 'which git'
                }
            }
        }
    }
}
