#!groovy
@Library('pipeline-library-demo@master')_

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
