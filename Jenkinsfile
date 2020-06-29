pipeline {
  agent any
  def mvnHome= tool name: 'Maven', type: 'maven'
  stages 
    {
    stage('Clean') {
      steps {
        sh '${mvnHome}/bin/mvn clean'
      }
    }
    stage('Compile') {
      steps {
        sh '${mvnHome}/bin/mvn compile'
      }
    }
    stage('Test') {
      steps {
        sh '${mvnHome}/bin/mvn test'
      }
    }
  }
}
