pipeline {
  agent any
  stages 
    {
    stage('Clean') {
      def mvnHome = tool name: 'Maven', type: 'maven'
      steps {
        sh '${mvnHome}/bin/mvn clean'
      }
    }
    stage('Compile') {
      def mvnHome = tool name: 'Maven', type: 'maven'
      steps {
        sh '${mvnHome}/bin/mvn compile'
      }
    }
    stage('Test') {
      def mvnHome = tool name: 'Maven', type: 'maven'
      steps {
        sh '${mvnHome}/bin/mvn test'
      }
    }
  }
}
