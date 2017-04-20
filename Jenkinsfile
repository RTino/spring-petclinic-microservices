pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        withMaven(maven: 'Maven 3.3.9') {
          sh 'mvn clean install -U -Dmaven.test.skip=true'
        }
        
      }
    }
  }
}