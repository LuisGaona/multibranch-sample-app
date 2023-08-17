pipeline {
  agent any
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
  }
}