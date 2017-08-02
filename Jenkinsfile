pipeline {
  agent none
  environment {
    MAJOR_VERSION=1
  }
  stages {
    stage('Learning Jenkins pipeline...') {
      agent any
        steps {
          sh 'ls -lhtra'
          sh 'pwd'
          sh 'git remote -v'
          sh 'git branch -a'
          sh 'printenv'
          sh 'echo "BUILD_URL variable data as found in the \'env\' variable is : ${BUILD_URL}"'
          mail to: 'pguddanti@nisum.com', subject: "[Testing]: Sending mail through Jenkinsfile build", body: "Testing..." //Mailing
        }
    }
  }
}
