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
            echo '"testing"'
          }
        }

        stage('Parallel') {
          steps {
            echo '"parallel running"'
          }
        }

      }
    }

    stage('Build Stage') {
      steps {
        echo '"Building"'
      }
    }

    stage('Clean Up') {
      steps {
        echo '"Clean Environment"'
      }
    }

  }
}