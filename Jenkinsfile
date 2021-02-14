pipeline {
  agent { label 'master' }
 
  stages {
    stage('Checkout code') { // clone the github code
      steps {
            checkout scm
      }
    }
    stage('Read YAML file') {
        steps {
            customWorkspace '/appl'
            script{ datas = readYaml (file: 'test.yml') }
            echo datas.ear_file.deploy.toString()

        }
    }
  }
}
