pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        withMaven(maven: 'Maven 3.1.1') {

          library 'Global Jenkins Lib'
          color_sh 'mvn install -Dmaven.test.skip=true'
        }
      }
    }
  }
}
