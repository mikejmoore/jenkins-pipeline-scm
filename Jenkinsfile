pipeline {
  agent none
  stages {
    stage('Test') {
      agent {
        docker { image 'mijomoore/http-responder:1.0'}
      }
      steps {
        sh 'ls /etc'
      }
    }
  }
}
