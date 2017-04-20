pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn install -Dmaven.test.skip=true'
        withMaven(maven: 'Maven 3.1.1')
      }
    }
  }
}