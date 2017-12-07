#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/Demo-prjt/demo1.git/'],
    pipelineTriggers (
        upstream(
   threshold: 'SUCCESS',
   upstreamProjects: 'https://github.com/Demo-prjt/demo1.git'
        ) )])
