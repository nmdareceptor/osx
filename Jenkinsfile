pipeline {
  agent any
  stages {
    stage('test hello') {
      parallel {
        stage('test hello') {
          steps {
            sh '''#!/bin/bash
                echo "hello this is my first test"'''
          }
        }
      }
    }
    stage('re-run') {
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
