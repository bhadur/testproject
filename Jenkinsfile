#!groovy
@Library('pipeline-library-demo@master')_

stage('Check Status') {
    helloWorld()
}

pipeline {
  agent { label 'master' }
 
  stages {
    stage('Call') { // clone the github code
      steps {
            helloWorld()
      }
    }
  }
}
