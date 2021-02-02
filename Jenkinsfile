pipeline {
  agent { label 'master' }
  stages {
    stage('Source') { // clone the github code
      steps {
        // clone code from our Github repository
        git 'https://github.com/bhadur/testproject'
      }
    }
