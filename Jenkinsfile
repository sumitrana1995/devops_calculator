node {
      stage('Clean') {
      def mvnHome = tool name: 'Maven', type: 'maven'
      
        sh '${mvnHome}/bin/mvn clean'
      
    }
    stage('Compile') {
      def mvnHome = tool name: 'Maven', type: 'maven'
      
        sh '${mvnHome}/bin/mvn compile'
      
    }
    stage('Test') {
      def mvnHome = tool name: 'Maven', type: 'maven'
      
        sh '${mvnHome}/bin/mvn test'
      
    }
}
