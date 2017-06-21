pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building..'
      }
    }
    stage('Test') {
      steps {
        echo 'Testing..'
      }
    }
    stage('Deploy') {
      steps {
        waitUntil() {
          input(message: 'Should we do this?', id: 'derp', ok: 'yes')
        }
        
      }
    }
    stage('Deploy2') {
      steps {
        echo 'Yeah buddy!'
      }
    }
  }
}