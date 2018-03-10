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
        stage('print') {
          steps {
            timeout(time: 3) {
              echo 'times up'
            }
            
          }
        }
        stage('retry') {
          steps {
            retry(count: 3)
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
}