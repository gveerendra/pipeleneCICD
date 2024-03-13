pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        echo 'This is Dev'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'This is Build'
          }
        }

        stage('Test') {
          steps {
            echo 'This is Test'
          }
        }

        stage('Prod') {
          steps {
            echo 'This is Prod'
          }
        }

      }
    }

  }
}