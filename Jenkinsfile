pipeline {
  agent {label 'windows'}
  options {
     buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')
    disableConcurrentBuilds()
  }
  stages {
    stage('hello') {
      steps {
        echo "hello"
      }
    }
    stage('cat README'){
      when{
       branch "fix-*"
      }
      steps{
       sh '''
           cat README.md
	  '''
      }
    }
  }
}
