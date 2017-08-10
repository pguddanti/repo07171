pipeline {
  agent none
  parameters {
    choice(name: 'pChoice1', choices: '1\n2\n3', description: 'Description for the param named Choice')
    choice(name: 'pChoice2', choices: '4\n5\n6', description: 'Description for the param named Choice')
    choice(name: 'pChoice3', choices: '7\n8\n9', description: 'Description for the param named Choice')
    booleanParam(name: 'bParam', defaultValue: true, description: 'Checkbox Parameter')
    string(name: 'fullName', defaultValue: 'G Prasanth Kumar', description: 'You can change the above full name')
  }
  environment {
    MAJOR_VERSION=1
  }
  stages {
    stage('Learning Jenkins pipeline...') {
      agent any
        steps {
          //sh 'ls -lhtra'
          //sh 'pwd'
          //sh 'git remote -v'
          //sh 'git branch -a'
          //sh 'printenv'
          //sh 'echo "BUILD_URL variable data as found in the \'env\' variable is : ${BUILD_URL}"'
          //mail to: 'pguddanti@nisum.com', subject: "[Testing]: Sending mail through Jenkinsfile build", body: "Testing..." //Mailing
          echo "Choice Selected: ${params.pChoice1}"
          echo "Choice Selected: ${params.pChoice2}"
          echo "Choice Selected: ${params.pChoice3}"
          echo "Boolean Selected: ${params.bParam}"
          echo "Name Entered: ${params.fullName}"
        }
    }
  }
}
