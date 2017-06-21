pipeline {
  agent any
  triggers {
    pollSCM('H/5 * * * *')
  }
  parameters {
    booleanParam(description: 'stuff', name: 'userFlag')
  }

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
