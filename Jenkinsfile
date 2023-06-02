pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'TEST'
          }
        }

        stage('Parallel') {
          steps {
            echo 'Parallel'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'Built/ Print messages'
      }
    }

    stage('Clean up') {
      steps {
        echo 'cleaning'
      }
    }

  }
  environment {
    Nack = 'docker'
  }
}