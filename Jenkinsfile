pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'make'
      }
    }
post {
        always {
            emailext body: 'A Test EMail', recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']], subject: 'Test'
        }
    }
  }
}
