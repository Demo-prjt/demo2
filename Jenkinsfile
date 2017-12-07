#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/Demo-prjt/demo2.git/'],
    pipelineTriggers (
        upstream(
   threshold: 'SUCCESS',
   upstreamProjects: 'https://github.com/Demo-prjt/demo1.git'
        ) )])


    stages {
        stage('Build') { 
            steps { 
                sh 'pwd' 
            }
        }
        stage('Test'){
            steps {
                sh 'java -version'
                
            }
        }
        stage('Deploy') {
            steps {
                sh 'ls'
                sh 'pwd'
            }
        }
    }
}
