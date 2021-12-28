pipeline {
  agent {
    label 'WORKSTATION'
  }

  triggers {
    pollSCM('*/2 * * * *')
  }

  stages {

    stage('Compile the Code') {
      steps {
        sh 'compile code'
      }
    }

    stage('Check the Code Quality') {
      steps {
        sh 'Check the code Quality'
      }
    }

    stage('Test Cases') {
      steps {
        sh 'Test Cases'
      }
    }

  }

}