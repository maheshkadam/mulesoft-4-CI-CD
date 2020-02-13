pipeline {
  agent any
  stages {
    stage('Unit Test') { 
      steps {
        bat 'mvn clean test'
      }
    }
    stage('Deploy CloudHub') { 
      steps {
        bat 'mvn deploy -P cloudhub -Dmule.version=4.2.2 -Danypoint.username=Man94 -Danypoint.password=Man@94' 
      }
    }
  }
}