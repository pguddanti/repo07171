pipeline {
  agent none
  environment {
    MAJOR_VERSION=1
  }
  stages {
    stage('listing directory contents') {
      agent any
        steps {
          sh 'ls -lhtra'
        }
    }
  }
}
