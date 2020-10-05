#!groovy
// first pipeline

properties([disableConcurrentBuilds()])

pipeline {
    agent {
        label 'master'
    }
    options {
        buildDiscarder(logRotator(numToKeepStr: '10', artifactNumToKeepsStr: '10'))
        timestapm()
        }
    stages {
        stage("step1") {
            steps
            {
                sh 'ssh root@10.0.0.20 \'uptime\''
            }
        }
    }    
    }
