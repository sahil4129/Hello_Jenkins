pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'make'
      }
    }
  }
  post {
    failure {
     mail(subject: 'Failure', body: 'Falite', from: 's.g.navingoyal@gmail.com', to: 'sahil@simyog.com')
    }
}
}
