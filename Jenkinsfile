pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
             date
           '''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing...'
          }
        }

        stage('Test Parallel') {
          steps {
            echo 'Test Parallel'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}