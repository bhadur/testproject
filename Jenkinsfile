#!/usr/bin/env groovy
@Library('pipeline-library-demo@master')_

configObj = ""

pipeline{
    agent any
    stages{    
        stage('prepare') {

    configObj = readYaml file : 'config/Test.yaml'

    flowManager  config : configObj
 }
        
}
}
