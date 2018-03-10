pipeline {
  agent any
  stages {
    stage('test hello') {
      parallel {
        stage('test hello') {
          steps {
            echo 'this is my first step'
          }
        }
      }
    }
    stage('status') {
      steps {
        echo 'success'
      }
    }
    stage('final') {
      steps {
        echo 'done'
      }
    }
  }
  environment {
    env = 'test'
  }
}