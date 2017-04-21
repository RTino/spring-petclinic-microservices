pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        (maven: 'Maven 3.3.9') {

          library 'Global Jenkins Lib'
          color_sh 'mvn install -Dmaven.test.skip=true'
        }
      }
    }
  }
}
