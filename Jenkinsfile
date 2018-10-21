pipeline {
  agent any
  stages {
    stage('one') {
      steps {
        sh 'echo "hello world!"'
      }
    }
    stage('second-all') {
      parallel {
        stage('second-1') {
          steps {
            echo 'bello!'
          }
        }
        stage('second-2') {
          steps {
            sh 'echo "second hi"'
          }
        }
      }
    }
  }
}