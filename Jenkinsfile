pipeline {
  agent any
  stages {
    stage('Exec') {
      steps {
        sh 'docker exec -u root -i toolkit_running ./usr/bin/apic'
        sh './usr/bin/apic yes no'
      }
    }
  }
}