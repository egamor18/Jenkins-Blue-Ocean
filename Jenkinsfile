pipeline {
  agent any
  stages {
    stage('first') {
      steps {
        echo 'hello this is the first stage'
      }
    }

    stage('second-stage') {
      parallel {
        stage('second-stage') {
          steps {
            echo 'this is the second stage'
          }
        }

        stage('parallel-stage') {
          steps {
            echo 'parallel stage mesage'
          }
        }

        stage('another-parallel-stage') {
          steps {
            echo 'another parallel stage'
          }
        }

      }
    }

    stage('third-stage') {
      steps {
        sh 'echo "this is the third stage"'
      }
    }

  }
  environment {
    label = 'python_agent'
  }
}