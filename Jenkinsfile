pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'make'
        catchError(catchInterruptions: true) {
          mail(subject: 'Failed', body: 'Pipeline  Failed ', to: 's.g.navingoyal@gmail.com', from: 'sahil@simyog.com')
        }

      }
    }

  }
}