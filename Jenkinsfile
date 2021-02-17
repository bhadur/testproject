#!/usr/bin/env groovy
@Library('pipeline-library-demo@master')_

def loadBranch(String branch) {
  //utils = load 'Jenkinsfiles/utils.groovy'
  if (fileExists("./Jenkinsfiles/default.yml")) {
    config = readYaml file: "./Jenkinsfiles/default.yml"
    println "config ==> ${config}"
  } else {
    config = []
  }

  if (config && config.pipeline && config.pipeline.enabled == false) {
    println "Pipeline disabled."
  } else {
     println "Pipeline enabled."
   
  }
}

node {
  stage("Prepare") {
    checkout scm
    sh 'git submodule sync'
    // Prepare for junit test results
    sh "mkdir -p test_results"
    sh "rm -f test_results/*.xml"

    // When checking in a file exists in another directory start with './' or
    // prepare to fail.
    loadBranch("default")
    
    
  }
}
