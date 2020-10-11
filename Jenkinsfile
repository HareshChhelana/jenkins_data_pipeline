pipeline {
  agent any
  stages {
    stage('Build') {
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
        sh '''echo "Script executed successfully"
echo "Script executed done"'''
        echo 'Deployment successfully completed.'
      }
    }

  }
}