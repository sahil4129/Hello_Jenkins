pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'make'
        mail(subject: 'fail', body: 'jhkh', to: 'sahil@simyog.com')
      }
    }

  }
}