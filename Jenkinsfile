pipeline {
    agent {
        dockerfile {
            filename 'Dockerfile'
            label 'label'
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
