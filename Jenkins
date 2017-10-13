pipeline {
    agent {
        docker {
            dockerfile 'Dockerfile'
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
