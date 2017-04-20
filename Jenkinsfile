pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        withMaven(maven: 'Maven 3.1.1') {
          sh 'mvn install -Dmaven.test.skip=true'
        }
        
      }
    }
  }
}