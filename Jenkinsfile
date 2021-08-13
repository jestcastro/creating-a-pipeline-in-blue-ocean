pipeline {
  agent any
  stages {
    stage('Create File') {
      steps {
        sh 'touch foo.bar'
      }
    }

    stage('LS files') {
      steps {
        sh 'ls'
      }
    }

    stage('docker') {
      steps {
        sh 'docker'
      }
    }

  }
}