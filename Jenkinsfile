pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Build successfully completed'
      }
    }

    stage('Test') {
      parallel {
        stage('Test 1') {
          steps {
            echo 'Test 1 successfully completed'
          }
        }

        stage('Test 2') {
          steps {
            echo 'Test 2 successfully completed'
          }
        }

        stage('Test 3') {
          steps {
            echo 'Test 3 successfully completed'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployment successfully completed.'
      }
    }

    stage('End') {
      steps {
        sh '''!#/bin/bash

echo "Data pipeline completed successfully"'''
      }
    }

  }
}