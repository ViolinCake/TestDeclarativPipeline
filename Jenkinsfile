pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed ...'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test completed ...'
          }
        }

        stage('Test2') {
          steps {
            echo 'hello from test2'
          }
        }

        stage('test3') {
          steps {
            echo 'hello from test3'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deployment completed ...'
      }
    }

  }
}