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

    stage('Deliver for development') {
        when {
            branch 'development'
        }
        steps {
            sh 'node -v'
        }
    }
    stage('Deploy for production') {
        when {
            branch 'master'
        }
        steps {
            sh 'ls'
        }
    }

  }
}