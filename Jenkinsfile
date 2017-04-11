pipeline {
  agent any
  stages {
    stage('DAC Desktop') {
      steps {
        parallel(
          "DAC Desktop": {
            build 'DAC - Desktop'
            
          },
          "": {
            build 'Smoke test - Thank page - Firefox - DDSTF002'
            
          }
        )
      }
    }
  }
}