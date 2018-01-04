
pipeline {
  agent none
  stages {
    stage('Build') {
      agent {
        docker { image 'mijomoore/http-responder:1.0'}
      }
      steps {
        echo 'Building....'
      }
    }
    stage('Unit Test') {
      agent {
        docker { image 'mijomoore/http-responder:1.0'}
      }
      steps {
        echo 'Unit Testing....'
      }
    }
    stage('UI Test') {
      agent {
        docker { image 'mijomoore/http-responder:1.0'}
      }
      steps {
        echo 'UI Testing....'
        sh 'ls /etc'
        sh 'curl localhost:3000'
        sh 'curl localhost:3000'
      }
    }
  }
}
