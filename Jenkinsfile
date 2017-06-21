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