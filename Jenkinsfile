pipeline {
  agent {label 'windows'}
  options {
    buildDiscarder logRotator(artifactDaysTokeepStr: '', artifactNumTokeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')
    disableCurrentBuilds()
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
