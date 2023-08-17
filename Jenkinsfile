pipeline {
  agent any
  options {
    buildDiscarder logRotator(artifactDaysTokeepStr: '', artifactNumTokeepStr: '5', daysTokeepStr: '', numTokeepStr: '5')
    disableConcurrentBuilds()
  }
  stages {
    stage('hello') {
      steps {
        echo "hello"
      }
    }
  }
}
