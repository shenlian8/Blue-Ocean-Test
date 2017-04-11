pipeline {
  agent any
  stages {
    stage('DAC Desktop') {
      steps {
        parallel(
          "DAC Desktop": {
            build 'UI - Smoke/DAC - Desktop'
            
          },
          "error": {
            build 'Smoke test - Thank page - Firefox - DDSTF002'
            
          }
        )
      }
    }
  }
}