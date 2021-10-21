pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'hello'
        sh 'echo "Second step"'
        sleep 1
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

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}