library 'Global Jenkins Lib'

pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
	withMaven(maven: 'Maven 3.3.9') {
          color_sh this 'echo test; mvn install -Dmaven.test.skip=true'
        }
      }
    }
  }
}
