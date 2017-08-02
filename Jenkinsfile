pipeline {
  agent none
  environment {
    MAJOR_VERSION=1
  }
  stages {
    stage('Executing some shell commands...') {
      agent any
        steps {
          sh 'ls -lhtra'
          sh 'pwd'
          sh 'git remote -v'
          sh 'git branch -a'
        }
    }
  }
}
