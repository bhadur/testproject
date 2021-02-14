def loadValuesYaml(){
  def valuesYaml = readYaml (file: './test.yml')
  return valuesYaml;
}

pipeline {
  agent {
    label "master"
  }

  environment {
    valuesYaml = loadValuesYaml()
  }
  stages {
    stage('CICD Initialize') {
      steps {
        script{
          echo valuesYaml
          println valuesYaml.getClass()
        }
        echo valuesYaml.appName.toString()
      }
    }
}
}
