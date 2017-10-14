#!/usr/bin/env groovy

projPath = 'src/github.com/tfgo-learn/jenkins-pipeline'

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
					sh "cd ${projPath} && pwd'
					sh 'pwd'
                	sh 'uname -a'
                	sh 'dep version'
                }
            }
        }
    }
}
