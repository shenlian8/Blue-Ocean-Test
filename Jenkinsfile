pipeline {
  agent any
  stages {
    stage('Stage 1') {
      steps {
        parallel(
          "Z1": {
            echo 'Hallo World!'
            
          },
          "Z2": {
            echo 'Hallo Z2'
            
          }
        )
      }
    }
  }
}