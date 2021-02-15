#!/usr/bin/env groovy
@Library('pipeline-library-demo@master')_

configObj = ""

pipeline{
    agent any
    stages {
        stage('Test') { // clone the github code
            steps {
            checkout scm
                configObj = readYaml file : 'config/Test.yaml'
                flowManager  config : configObj
            }
        }
    }
