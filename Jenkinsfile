pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'hello'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sh 'python --version'
          }
        }

        stage('Test1') {
          steps {
            echo 'test'
          }
        }

      }
    }

  }
}