pipeline {
  agent any
  stages {
    stage('checkout code') {
      steps {
        git(url: 'https://github.com/farheen0204/GItHub', branch: 'master')
      }
    }

    stage('log') {
      steps {
        sh 'ls -al'
      }
    }

    stage('build') {
      steps {
        sh 'docker build -f /Users/arpitkhare/.jenkins/workspace/Dockerfile .'
      }
    }

  }
}