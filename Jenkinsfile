pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building..'
        sleep 10
      }
    }
    stage('Test') {
      steps {
        echo 'Testing..'
        sleep 10
      }
    }
    stage('Deploy Check') {
      steps {
        input(message: 'Should we do this?', id: 'check', ok: 'YES!')
      }
    }
    stage('Deploy2') {
      steps {
        echo 'Yeah buddy!'
      }
    }
  }
}