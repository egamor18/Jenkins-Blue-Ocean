pipeline {
  agent any
  stages {
    stage('first') {
      steps {
        echo 'hello this is the first stage'
      }
    }

    stage('second-stage') {
      steps {
        echo 'this is the second stage'
      }
    }

    stage('third-stage') {
      steps {
        sh 'echo "this is the third stage"'
      }
    }

  }
}