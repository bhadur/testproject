#!/usr/bin/env groovy
@Library('pipeline-library-demo@master')_



pipeline{
    agent any
    stages {
        stage('Test') { // clone the github code
            steps {
            
                def datas = readYaml file: 'config/Test.yaml', text: "something: 'Override'
                flowManager  config : datas
            }
        }
    }
}
