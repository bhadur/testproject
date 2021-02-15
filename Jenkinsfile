#!/usr/bin/env groovy
@Library('pipeline-library-demo@master')_

configObj = ""

pipeline{
    ...
script{

    configObj = readYaml file : 'config/Test.yaml'

    flowManager  config : configObj
 }
       ...    
}
