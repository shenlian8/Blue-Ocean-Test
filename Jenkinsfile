pipeline {
  agent any
  stages {
    stage('1. Stage') {
      steps {
        parallel(
          "DAC Desktop": {
            build 'UI - Smoke/DAC - Desktop'
            
          },
          "Thanks page 002": {
            build 'Smoke test - Thank page - Firefox - DDSTF002'
            
          }
        )
      }
    }
    stage('Input') {
      steps {
        input(message: 'm', id: 'i', ok: 'ok', submitter: 's', submitterParameter: 'p')
      }
    }
  }
}