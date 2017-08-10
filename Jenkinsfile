pipeline {
  agent none
  parameters {
    choice(name: 'pChoice', choices: 'One\nTwo\nThree', description: 'Description for the param named Choice')
    booleanParam(name: 'bParam', defaultValue: true, description: 'Checkbox Parameter')
  }
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
          //mail to: 'pguddanti@nisum.com', subject: "[Testing]: Sending mail through Jenkinsfile build", body: "Testing..." //Mailing
          echo "Choice Selected: ${params.pChoice}"
          echo "Boolean Selected: ${params.bParam}"
          //echo "Name Entered: ${params.fullName}"
        }
    }
  }
}
