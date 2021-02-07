#!groovy
@Library('pipeline-library-demo@master')_

pipeline {
  agent { label 'master' }
 
  stages {
    stage('Checkout code') { // clone the github code
      steps {
            checkout scm
      }
    }
  }
}
