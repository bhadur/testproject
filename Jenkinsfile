pipeline {
  agent { label 'master' }
  libraries {
        lib('pipeline-library-demo')
        }  
  stages {
    stage('Checkout code') { // clone the github code
      steps {
            checkout scm
      }
    }
  }
}
