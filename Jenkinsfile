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

    stage('sh') {
      steps {
        sh 'node -v'
      }
    }

    stage('yarn') {
      steps {
        sh '''sudo mkdir /var/builds/
cd ~/var/builds/
pwd
ls'''
      }
    }

  }
}