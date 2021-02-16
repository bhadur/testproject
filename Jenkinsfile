pipeline {
  agent {
    label "master"
  }
  
  stages {
    stage ('Check logs') {
    datas = readYaml file: "test.yml"
    }
  }

}

 
