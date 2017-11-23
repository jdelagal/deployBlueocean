pipeline {
  agent any
  stages {
    stage('Exec') {
      steps {
        sh 'docker exec -u root -i toolkit_running bash'
        sh './usr/bin/apic yes no'
      }
    }
  }
}