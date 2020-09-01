pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'make'
        catchError(catchInterruptions: true) {
          mail(subject: 'Failure', body: 'Falite', from: 's.g.navingoyal@gmail.com', to: 'sahil@simyog.com')
        }

      }
    }

  }
}