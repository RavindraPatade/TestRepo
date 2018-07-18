pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('Build') {
      agent any
      steps {
        bat(script: 'test.bat', returnStatus: true)
        mail(subject: 'TESTMAIL', body: 'TESTING', to: 'ravindrapatade@gmail.com')
      }
    }
  }
}