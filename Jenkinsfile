@Library('Global Jenkins Lib') import static com.foo.Utilities.*
node {
    stage('Checkout and Build') {
        checkout scm
        wrap([$class: 'AnsiColorBuildWrapper', 'colorMapName': 'XTerm']) {
	    color_sh this 'echo test; mvn install -Dmaven.test.skip=true'
        }
    }
}
