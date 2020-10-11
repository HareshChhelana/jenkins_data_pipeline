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
            echo 'Test successfully completed'
          }
        }

        stage('Sub test 1') {
          steps {
            echo 'Sub test 1 successfully completed'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployment successfully completed.'
      }
    }

  }
}