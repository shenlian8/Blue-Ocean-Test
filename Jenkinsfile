pipeline {
  agent any
  stages {
    stage('Input') {
      steps {
        timeout(unit: 'MINUTES', time: 2) {
          input(message: 'Hi, input', id: 'userInput', ok: 'OK', submitter: 's', submitterParameter: 'p')
        }
        
      }
    }
  }
}