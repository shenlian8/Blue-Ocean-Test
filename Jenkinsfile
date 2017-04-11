pipeline {
  agent any
  stages {
    stage('1') {
      steps {
        parallel(
          "1": {
            echo 'Hallo World'
            echo 'Hallo 2'
            
          },
          "1.1": {
            echo 'Hallo 1.1'
            
          }
        )
      }
    }
    stage('2') {
      steps {
        echo 'Hallo Step 2'
      }
    }
  }
  environment {
    a = 'a'
    b = 'b'
  }
}