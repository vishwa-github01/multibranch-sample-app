pipeline {
  // agent {label 'linux'}
  agent any
  options {
    buildDiscarder(logRotator(numToKeepStr: '5'))
  }
  stages {
    stage('Build') {
      steps {
        echo "Hello this is Build stage"
        // sh './gradlew clean check --no-daemon'
      }
    }
  }
  // post {
  //   always {
  //       junit(
  //         allowEmptyResults: true, 
  //         testResults: '**/build/test-results/test/*.xml'
  //       )
  //   }
  // }
}
