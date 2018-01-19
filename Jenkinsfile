pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('build') {
          steps {
            echo 'Building..'
          }
        }
        stage('test') {
          steps {
            echo 'Testing..'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }
    stage('Input') {
      steps {
        input 'looking good?'
      }
    }
    stage('Finish') {
      steps {
        echo 'yay'
      }
    }
  }
}