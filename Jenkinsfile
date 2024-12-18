pipeline {
  agent any
  stages {
    stage('Commit stage') {
      steps {
        echo 'Hi this is commit stage'
      }
    }

    stage('Build stage') {
      steps {
        echo 'Hi this is build stage'
      }
    }

    stage('test') {
      steps {
        echo 'Hi this is test stage'
      }
    }

    stage('Staging') {
      steps {
        echo 'Hi this is staging'
      }
    }

    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            echo 'Hi this is deploy stage'
          }
        }

        stage('Operate') {
          steps {
            echo 'Hi this is operate stage'
          }
        }

      }
    }

  }
}